# quiz_app

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.



## backend

mkdir backend
cd backend
python3 -m venv venv
source venv/bin/activate
pip install django djangorestframework
django-admin startproject [name] .
python manage.py startapp quiz
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
python manage.py createsuperuser
