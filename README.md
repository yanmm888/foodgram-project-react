# Yamdb with Docker and workflows
## База отзывов пользователей о фильмах, музыке и книгах
## Стек технологий: Python 3, Django REST Framework, PostgreSQL, Simple-JWT, NGINX, Docker, flake, pytest
### Проект развернут на http://foodgram.ps-card.ru
### Статус workflow: 
![example workflow](https://github.com/yanmm888/foodgram-project-react/actions/workflows/foodgram_workflow.yaml/badge.svg)
____
##### Создание файла с переменными окружения .env
Пример:
- Ключ приложения ```SECRET_KEY='very_strong_secret_key'```
- выбор движка СУБД ```DB_ENGINE=django.db.backends.postgresql```
- название базы ```DB_NAME=postgres```
- имя пользователя базы ```POSTGRES_USER=postgres```
- пароль базы данных ```POSTGRES_PASSWORD=postgres```
- адрес базы ```DB_HOST=db``` 
- порт базы```DB_PORT=5432```


### Запуск приложения:
```docker-compose up```

### Выполнить миграции:
```docker-compose exec backend python manage.py migrate``` 

### Создать суперпользователя:
```docker-compose exec backend python manage.py createsuperuser```
#### для windows 
```winpty docker-compose exec backend python manage.py createsuperuser```

#### Загрузка ингридиентов
```docker-compose exec backend python manage.py load_ingredients```

### Информация об образе на Dockerhub
```nmm888/foodgram```
### Информация об авторе
Malik Nurmagomedov
```https://github.com/yanmm888/```
