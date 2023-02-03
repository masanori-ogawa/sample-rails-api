# README

## 環境構築

- `/rails-app-dirname`で全検索し作成したディレクトリ名に変更する
- `docker-compose.yml`のコンテナ名を変更する（sample*rails_app*を作成するアプリ名に変更）
- `docker compose build --no-cache`
- `docker compose up -d`
- `docker compose exec app rails db:create`:DB 作成
- `yarn`: prettier インストール（デフォルトフォーマッタを prettier に設定）
- `http://localhost`にアクセス

## rails コマンド実行

- `docker compose run --rm app bundle exec rails xxx`
- `docker-compose run --rm api bundle exec rails db:migrate` マイグレーション
- `docker-compose run --rm api bundle exec rails db:seed` seeder 実行

## Rubocop を有効にする

https://qiita.com/k_kuma/items/304cfe373981e956e2bb
