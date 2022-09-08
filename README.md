# Django-Base-Project

This repository includes basic django structure.

### Branch: `main`

- `.gitignore` file for django project.
- Main project folder is `core`.
- `requirements.txt` file with `django` and `python-dotenv` in it.

### Branch: `accounts`

- All features of `main` branch.
- `accounts` app installed and configured with corresponding model and model manager.
- This accounts app is specific for changing USERNAME_FIELD from `username` to `email`.

## To use accounts app

### To install redis server
    sudo apt install redis

### To start redis server
    redis-server

### To install redis server
    service redis-server stop

### To restart redis server
    service redis-server restart

### To check status of redis server
    service redis-server status

### To start celery
    celery -A core worker --pool=solo -l info
    celery -A core worker -l info
    celery -A core worker