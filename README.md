git clone https://github.com/sashabizoo/test_env1.git

cd test_env1

смотрим настройки окружения в файле .env, и если надо меняем

DB_CONNECTION=mysql
DB_HOST=mysql
DB_USERNAME=root
DB_PASSWORD=password
DB_DATABASE=laravel_test

docker compose up -d
