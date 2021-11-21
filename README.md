# DNLVP
Dockerを使用してローカルに、
Nginx, Laravel(PHP), VueJS, PostgresSQLの開発環境を作るための設定ファイルです。
C
onfig files are for build local development environment(Nginx, Laravel(PHP), VueJS, PostgresSQL) by Docker.

# Note
ローカルでのDockerコマンド実行前に、
`docker-compose.yml`内の`pgadmin`の`environment`の`PGADMIN_DEFAULT_EMAIL`のメールアドレスを適宜変更してください。

また、`docker/web/default.conf`内にて、
rootを`root /var/www/html/[dnlvp]/public;`と指定しています。

作成するLaravelのプロジェクト名(フォルダ名)に合わせて[dnlvp]の部分を変更してください。


Please change mail address wrote `PGADMIN_DEFAULT_EMAIL` 
in `docker-compose.yml` file at `pgadmin` in `environment` before you execute Docker command at your local.

Root document has set `root /var/www/html/[dnlvp]/public;` in `docker/web/default.conf`.
Please change [dnlvp] to your Laravel project(folder) name.

# Requirement
Docker version 20.10.10
 
# Installation
git clone https://github.com/roughstorm/dnlvp
cd dnlvp
docker-compose up --build -d