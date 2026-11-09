# Django Discussion Board

> A forum web app built with Django and PostgreSQL: boards, topics and threaded replies, with user accounts.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?logo=bootstrap&logoColor=white)

## Features

- **Boards:** the admin creates discussion boards from the Django admin.
- **Topics and posts:** signed-in users start topics, reply to them, and edit their own posts. Each topic tracks its view count.
- **Accounts:** sign up, log in and out, change password, and edit the account page.
- **Clean structure:** two apps (`boards`, `accounts`), class- and function-based views, and Django forms styled with `django-widget-tweaks`.

## Data model

`Board` 1 ─── * `Topic` 1 ─── * `Post`, and each topic and post belongs to a `User`.

## Run it

```bash
git clone https://github.com/AhmedGamal98/django-discussion-board.git
cd django-discussion-board
pip install -r requirements.txt

# settings are read from environment variables
export DJANGO_SECRET_KEY="change-me"
export DB_NAME=boards_django DB_USER=postgres DB_PASSWORD=your_password

python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

On Windows PowerShell, set the variables with `$env:DB_PASSWORD = "your_password"` and so on.

## Author

**Ahmed Gamal Saber**, Full-Stack Web Developer & AI Engineer
[LinkedIn](https://linkedin.com/in/ahmed-gamal-saber-382081169) · [GitHub](https://github.com/AhmedGamal98)
