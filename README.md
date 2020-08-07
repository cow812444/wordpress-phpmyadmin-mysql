# wordpress-phpmyadmin-mysql
1.docker-compose up -d,等待执行完成

2.外网可通过vps的ip地址+端口访问phpmyadmin管理页面与wordpress。

：phpmyadmin登录帐号和密码使用前面的WORDPRESS_DB_USER和WORDPRESS_DB_PASSWORD。

：mysql数据库密码不能用特殊字符，否则数据库可能会无法启动，phpmyadmin登录也就会失败。

3.宿主机(vps)安装nginx，实现域名与容器应用实例的映射。

4.域名要提前备好，并再dns中设置。

5.将nginx.conf的文件放到/etc/nginx/conf.d/ 目录下，文件名不限。
