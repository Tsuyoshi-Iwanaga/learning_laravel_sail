# Laravel

## Laravel Sailを経由してセットアップ
Laravel SailはDockerでの構築を簡単にできるツール
下記2コマンドでアプリの立ち上げまで動作する

```
curl -s https://laravel.build/example-app | bash
```

```
cd example-app && ./vendor/bin/sail up -d
```

※ 上記コマンドのexample-appは任意のディレクトリ名

## 立ち上がるコンテナ

laravel.test_1 (※ポート80)
mailhog_1
meilisearch_1
mysql_1
redis_1
selenium_1

## 通常時のコマンド

立ち上げ

```
./vendor/bin/sail up -d
```

終了

```
./vendor/bin/sail down
```

ステータス確認

```
./vendor/bin/sail ps
```

アプリコンテナに入る(artisanの実行など)

```
./vendor/bin/sail shell
```

MySQLコンテナに入る

```
./vendor/bin/sail mysql
```