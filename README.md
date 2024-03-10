
アプリ名　勤怠管理システム

作成した目的

勤怠の管理を楽にするため

アプリケーションURL


機能一覧
ログイン機能
新規登録機能
ログアウト機能

使用技術
laravel 8.83.8

テーブル設計
https://github.com/mikage123/Atte-form/assets/149714537/87703e56-7e7a-4826-97c4-e82624b368db

ER図
(https://github.com/mikage123/Atte-form/assets/149714537/200592fa-dbdb-4e94-bb01-018cee96a013)

環境構築
git@github.com:mikage123/Atte-form.git

docker-compose up -d --build

docker-compose exec php bash

composer install

.env.exampleファイルから/envを作成し、環境変数を変更

.envに以下の環境変数を追加

DB_CONNECTION=mysql

DB_HOST=mysql

DB_PORT=3306

DB_DATABASE=laravel_db

DB_USERNAME=laravel_user

DB_PASSWORD=laravel_pass

アプリケーションキーを作成

php artisan key:generate

開発環境:http://localhost/

phpmyadmin:http://localhost:8080/
