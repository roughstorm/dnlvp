# DNLVP
Dockerを使用してローカルに、<br>
Nginx, Laravel(PHP), VueJS, PostgresSQLの開発環境を作るための設定ファイルです。<br>
<br>
Config files are for build local development environment(Nginx, Laravel(PHP), VueJS, PostgresSQL) by Docker.<br>

# Note
ローカルでのDockerコマンド実行前に、<br>
`docker-compose.yml`内の`pgadmin`の`environment`の`PGADMIN_DEFAULT_EMAIL`のメールアドレスを適宜変更してください。<br>
<br>
また、`docker/web/default.conf`内にて、<br>
rootを`root /var/www/html/[dnlvp]/public;`と指定しています。<br>
<br>
作成するLaravelのプロジェクト名(フォルダ名)に合わせて[dnlvp]の部分を変更してください。<br>
<br>
<br>
Please change mail address wrote `PGADMIN_DEFAULT_EMAIL` <br>
in `docker-compose.yml` file at `pgadmin` in `environment` before you execute Docker command at your local.<br>
<br>
Root document has set `root /var/www/html/[dnlvp]/public;` in `docker/web/default.conf`.<br>
Please change [dnlvp] to your Laravel project(folder) name.<br>
<br>

# Requirement
Docker version 20.10.10
 
# Installation
git clone https://github.com/roughstorm/dnlvp
cd dnlvp
docker-compose up --build -d