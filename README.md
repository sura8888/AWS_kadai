*URL乗せ忘れたためここに記述*
(http://3.93.174.83/AWS_Kadai.php)

docker compose up　でdockerを起動

*テーブルをMySQLに作成*
```
docker compose exec mysql mysql kyototech
```

MySQLクライアントを起動したら以下のSQLを実行し、テーブルを作成
```
CREATE TABLE `logs` (
    `id` INT AUTO_INCREMENT PRIMARY KEY,
    `text` TEXT NOT NULL,
    `created_at` DATETIME DEFAULT CURRENT_TIMESTAMP
);
```
