Окружение Nginx + PHP + MySQL

Установка

1. Клонируем окружение. Делаем команду (на выбор):

git clone git@github.com:sashabizoo/laravel_env1.git  
или 
git clone https://github.com/sashabizoo/laravel_env1.git

2. Заходим в созданную папку

cd laravel_env1

3. Смотрим настройки окружения в файле .env, имена, порты и если надо меняем

Настройки Mysql сервера:

DB_CONNECTION=mysql
DB_HOST=mysql
DB_USERNAME=root
DB_PASSWORD=password
DB_DATABASE=laravel_test
DB_PORT=3306

MYSQL_PORT=3316 - внешний порт Mysql
HTTP_PORT=8889 - внешний порт Http

4. Для поднятия окружения делаем команду

Для Linux: docker-compose up -d

Для Mac OS: docker compose up -d

5. Для того чтобы остановить и удалить все контейнеры, тома и образы делаем команду

Для Linux: docker-compose down -v

Для Mac OS: docker compose down -v
