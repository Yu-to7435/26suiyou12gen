## 手順書

## リポジトリクローン

git clone https://github.com/Yu-to7435/26suiyou12gen.git

## dockerコンテナの新規起動

docker compose up -d --build

## docker新規起動後

docker compose upでよい。

## mysqlコンテナ

docker compose exec mysql mysql example_db

## データベース作成

CREATE TABLE `bbs_entries` (
    `id` INT UNSIGNED NOT NULL AUTO_INCREMENT PRIMARY KEY,
    `body` TEXT NOT NULL,
    `created_at` DATETIME DEFAULT CURRENT_TIMESTAMP,
    `image_filename` TEXT DEFAULT NULL
);


## webアプリにアクセス

http://<ec2のipアドレス>/kadai.php


