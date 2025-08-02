# Пульт охраны банка

Это внутренний репозиторий для сотрудников банка «Сияние». Если вы попали в этот репозиторий случайно, то вы не сможете его запустить, т.к. у вас нет доступа к БД, но можете свободно использовать код или изучить реализацию запросов к БД.

## Установка и запуск

1. Склонируйте репозиторий:
   ```bash
   git clone [ваш-repo-адрес]

2. Убедитесь, что у вас установлен Python 3.8+
3. Установите зависимости:
   ```bash
   pip install -r requirements.txt

4. Создайте .env файл (запросите актуальные данные у администратора):
    ```ini
    DB_ENGINE=django.db.backends.postgresql
    DB_HOST=ваш_хост
    DB_PORT=ваш_порт
    DB_NAME=имя_бд
    DB_USER=ваш_логин
    DB_PASSWORD=ваш_пароль
    SECRET_KEY=ваш_секретный_ключ

### Описание переменных окружения

`DB_ENGINE` Движок базы данных (для PostgreSQL используйте `django.db.backends.postgresql`) [ENGINE](https://docs.djangoproject.com/en/5.2/ref/settings/#engine)

`DB_HOST`	Адрес сервера базы данных [Host](https://docs.djangoproject.com/en/5.2/ref/settings/#host)

`DB_PORT`	Порт подключения к БД (по умолчанию 5432 для PostgreSQL) [PORT](https://docs.djangoproject.com/en/5.2/ref/settings/#port)

`DB_NAME`	Имя базы данных [NAME](https://docs.djangoproject.com/en/5.2/ref/settings/#name)

`DB_USER`	Пользователь БД [USER](https://docs.djangoproject.com/en/5.2/ref/settings/#user)

`DB_PASSWORD`	Пароль пользователя БД [PASSWORD](https://docs.djangoproject.com/en/5.2/ref/settings/#password)

`SECRET_KEY`	Криптографический ключ для защиты Django. Должен быть уникальным! [SECRET_KEY](https://docs.djangoproject.com/en/5.2/ref/settings/#secret-key)

## Что делать, если нет доступа к БД
1. Изучите код работы с Django ORM
2. Можете заменить настройки в .env на тестовую БД

## Запуск
```bash
   python main.py