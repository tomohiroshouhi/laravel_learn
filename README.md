# 立ち上げ
docker-compose up -d
# 関連ライブラリのインストール
docker-compose exec laravel-app composer install
# テーブル作成
docker-compose exec laravel-app php artisan migrate

# db 接続情報
どっかーを起動後、テーブル作成コマンドを実行し以下の情報を各SQLエディタに入力

Host> localhost:11306
Database> app
User> root
Password> root

※　この情報はdocker-compose.ymlファイルに記載