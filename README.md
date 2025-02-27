# お問い合わせフォーム
## 環境構築
1 git clone ()
2 docker-compose up -d --build
3 docker-compose exec php bash
4 composer install
5 cp .env.example .env
  データベースの環境変数を変更

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=laravel_db
DB_USERNAME=Laravel_user
DB_PASSWORD=Laravel_pass

6 php artisan key:generate
7 php artisan migrate
8 php artisan db:seed

## 使用技術(実行環境)
・ nginx 1.21.1 

・ php 7.4.9

・ MySQL 8.0

・laravel 8.83

## ER図
/Users/miki/coachtech/test-contact/contact-form/contact.drawio.png

## URL
・開発環境:http://localhost/

・phpMyAdmin:http://localhost:8080/
