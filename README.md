# php7-fpm_nginx_mariadb

# req
docker && docker-compose

# run
git clone.. cd to project folder,
run nginx_cert_selfsign.sh for generate ssl certificate for nginx container.
run docker-compose up -d 
run install_pdo_mysqli.sh for compile pdo-mysqli ext in php7_fpm container.

if u use centos 7 with selinux, use this:
chcon -Rt svirt_sandbox_file_t /path_to_folders_db
