# Окружение Nginx + PHP + MySQL

## Установка

### Клонируем окружение. Делаем команду (на выбор):

git clone git@github.com:sashabizoo/laravel_env1_maketest.git 

### Заходим в созданную папку

cd laravel_env1_maketest

### Смотрим настройки окружения в файле .env, имена, порты и если надо меняем

## Настройки Mysql сервера:

DB_CONNECTION=mysql

DB_HOST=mysql

DB_USERNAME=root

DB_PASSWORD=password

DB_DATABASE=laravel_test

DB_PORT=3306

L5_SWAGGER_CONST_HOST=http://localhost:8889 - локальный хост и порт для Swagger open API

MYSQL_PORT=3316 - внешний порт Mysql
HTTP_PORT=8889 - внешний порт Http

## Для поднятия окружения делаем команду

### Для Linux:

docker-compose up -d

### Для Mac OS: 

docker compose up -d

## Для того чтобы остановить и удалить все контейнеры, тома и образы делаем команду

### Для Linux: 

docker-compose down -v

### Для Mac OS: 

docker compose down -v

## Для остановки с удалением всех контейнеров, томов, образов и сборок

### Для Linux: 

docker-compose down -v --rmi all --remove-orphans

### Для Mac OS: 

docker compose down -v --rmi all --remove-orphans
