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

pip install django-cors-headers gunicorn psycopg2-binary whitenoise dj-database-url

django-cors-headers : 코스 에러 방지
gunicorn : 배포 툴
psycopg2-binary, dj-database-url : heroku에서 사용하는 db인  postgresql을 사용하기 위한 패키지
whitenoise : 정적 파일의 사용을 돕는 미들웨어


pip freeze > requirements.txt

brew install heroku/brew/heroku : 헤로쿠 cli 설치

heroku login

heroku create [name]


<!-- heroku git:remote -a drf-quiz-app (최상위 루트에 생성해야 함) -->

git push heroku master

heroku run python manage.py migrate

heroku run python manage.py createsuperuser

