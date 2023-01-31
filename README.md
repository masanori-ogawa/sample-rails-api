# README

## 環境構築
 - `/rails-app-dirname`で全検索し作成したディレクトリ名に変更する
 - `docker-compose.yml`のコンテナ名を変更する（sample_rails_app_を作成するアプリ名に変更）
 - `docker compose build --no-cache`
 - `docker compose up -d`
-  `docker compose exec app rails db:create`：DB作成
- `http://localhost`にアクセス

## railsコマンド実行
`docker compose run --rm app bundle exec rails xxx`
`docker-compose run --rm api bundle exec rails db:migrate` マイグレーション
`docker-compose run --rm api bundle exec rails db:seed` seeder実行