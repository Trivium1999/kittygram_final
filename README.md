[![Build Status](https://github.com/Trivium1999/kittygram_final/workflows/main.yml/badge.svg)](https://github.com/Trivium1999/kittygram_final/actions/workflows/main.yml)
<code>if (condition) {
[![Build Status](https://github.com/Trivium1999/kittygram_final/workflows/Main/badge.svg)](https://github.com/Trivium1999/kittygram_final/actions/workflows/Main.yml)
}</code>
[![Build Status](https://github.com/Trivium1999/kittygram_final.svg?branch=main)](https://travis-ci.com/username/projectname)

#  Kittygram
Блог для любителей котиков. Можно добавлять фото, имя, цвет и достижения любимых питомцев.

![example workflow](https://github.com/github/docs/actions/workflows/main.yml/badge.svg)
#  В проекте были использованы технологии:
- Django REST
- Python 3.9
- Gunicorn
- Nginx
- JS
- Node.js
- PostgreSQL
- Docker

#  Запуск проекта из репозитория GitHub:
1. Клонируйте репозиторий на свой компьютер
2. Запустите:
```
sudo docker compose -f docker-compose.yml up -d
```

# Запуск проекта из образов DockerHub:
1. Создайте папку, в которой будет храниться проект
2. Скачайте файл ```docker-compose.production.yml``` и запустите его командой:
```
sudo docker compose -f docker-compose.yml up -d
```

### Миграции:
```
sudo docker compose -f [имя-файла-docker-compose.yml] exec backend python manage.py migrate
```
### Сбор статики:
```
sudo docker compose -f [имя-файла-docker-compose.yml] exec backend python manage.py collectstatic

sudo docker compose -f [имя-файла-docker-compose.yml] exec backend cp -r /static/. /backend_static/static/
```

##  Остановка контейнеров:
```
sudo docker compose -f docker-compose.yml down
```

## Автор(devops)
Анна Романова
