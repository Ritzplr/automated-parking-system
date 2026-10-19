# Automated Parking System

A Django web app for managing parked vehicles and parking slots, with a shortest-distance calculation between parking spaces.

## Features

- Sign up and sign in
- Record a parked vehicle: state, vehicle number, vehicle type, date, time and price (default 20)
- Parking spaces with coordinates and individual slots that track whether they are vacant
- Distances between spaces, with a shortest-path helper (`parking_app/utils.py`) exposed at `/calculate-shortest-distance/` as a demo

## Stack

Python, Django, HTML, CSS, JavaScript, SQLite

## Run locally

```bash
pip install django
python manage.py migrate
python manage.py runserver
```

Open http://127.0.0.1:8000/.

## Layout

| Path | Purpose |
|---|---|
| `parking_system/` | Django project settings and root URLs |
| `parking_app/` | Models, views, URLs and the shortest-distance utility |
| `templates/`, `static/` | HTML templates and static files |
