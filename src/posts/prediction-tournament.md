---
title: "Building a Prediction Tournament Web App on Raspberry Pi"
emoji: ⚽
date: 2025-9-26T16:59:33.310Z
summary: "Building a Prediction Tournament Web App on Raspberry Pi"
metaDescription: "Building a Prediction Tournament Web App on Raspberry Pi"
tags:
  - Flask
  - SQLite
  - python
  - Raspberry
  - BeautifulSoup
  - Linux
---
One of my recent projects was to design and deploy a football prediction tournament platform. The goal was to let a group of friends compete against each other by predicting the outcomes of local football leagues, tracking their scores, and displaying live leaderboards. What makes this project special is that it’s not hosted in the cloud, it runs entirely on my own Raspberry Pi, exposed securely to the internet.

At the heart of the application is Flask. A lightweight Python web framework. Flask was the perfect choice because it is simple, flexible, and easy to extend.
Routing: Flask handles user interactions, such as logging in, submitting predictions, and viewing leaderboards.
Authentication: I used Flask-Login to manage sessions, with support for admin users who can edit match schedules.
Database ORM: For persistence, I used Flask-SQLAlchemy, an Object Relational Mapper (ORM) built on top of SQLAlchemy. This makes database queries both powerful and Pythonic.

The data model includes several tables:
calendario for official match schedules and results, giocatore for users, pronostico for predictions, partita and classification tables to track tournament standings.

Because this project is designed for a small community, I chose SQLite as the database. It’s lightweight, requires no server setup, and integrates seamlessly with SQLAlchemy. The simplicity of a single .sqlite file also makes backups and migrations straightforward.

![](/src/assets/img/pronostici.jpeg)

For the UI, I relied on:
Jinja2: templating (integrated with Flask) to render HTML pages with dynamic content.
Bootstrap 5: for responsive layouts, ensuring the site works well on both desktop and mobile.
Custom CSS: to highlight correct/incorrect predictions with color coding and to display player logos next to their names.

Match results are automatically updated by scraping official league websites. I built Python scripts with:
Requests, BeautifulSoup4 (bs4) and optionally lxml for fast HTML parsing.
These scripts populate the calendario table with live results, which then trigger the scoring logic for predictions and head-to-head matchups.

Instead of using a cloud server, I deployed the platform on a Raspberry Pi running Rasppberry OS:
Gunicorn serves the Flask app in production.
Nginx acts as a reverse proxy, handling HTTP requests, serving static files (images, logos, CSS), and forwarding dynamic requests to Gunicorn.
Let’s Encrypt + Certbot provides free HTTPS certificates, securing communication even over the public internet.

To keep everything up to date, I configured scheduled tasks with cron on the Raspberry Pi
