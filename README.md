Gas Service Request System - Setup Guide

This guide will help you set up and run the Gas Service Request System on your local machine.

📌 Introduction

The Gas Service Request System is designed to allow customers to submit and track service requests related to gas utility services. The system provides an admin panel for managing service requests and user authentication for secure access.

📌 Prerequisites

Before running the project, ensure you have the following installed:

Python (>= 3.8)

Django (>= 4.0)

SQLite (default Django database)
Routes Overview
http://127.0.0.1:8000/requests/track/      || Track the status of submitted requests
http://127.0.0.1:8000/requests/submit/     || Submit a new gas service request
http://127.0.0.1:8000/admin/               || Admin panel

Project Structure

gas_service/  <-- Main project directory
│── gas_service/      <-- Main Django app
│   ├── settings.py
│   ├── urls.py
│   ├── views.py
│   ├── models.py
│   ├── templates/
│   │   ├── base.html
│   │   ├── registration/login.html
│   │   ├── service_requests/submit_request.html,track_requests.html
│── service_requests/ <-- App handling customer requests
│   ├── urls.py
│   ├── views.py
│   ├── models.py
│   ├── templates/service_requests/
│── manage.py
│── db.sqlite3
│── venv/ (virtual enviornment optional)
