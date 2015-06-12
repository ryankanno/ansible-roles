# nginx

This role installs [nginx](http://nginx.org).

## role variables

|name|description|default|
|----|-----------|-------|
|`nginx.package`|nginx package|nginx|
|`nginx.version`|nginx package version|1.8.0-1~trusty|
|`nginx.config.src`|path to nginx config|nginx.conf.j2|
|`nginx.config.vars.user`|nginx user|www-data|
|`nginx.config.vars.pid`|nginx pid|/var/run/nginx.pid|
|`nginx.config.vars.max_clients`|nginx max client|8096|
|`nginx.config.vars.access_log`|nginx access log|/var/log/nginx/access.log|
|`nginx.config.vars.error_log`|nginx error log|/var/log/nginx/error.log|
|`env`|dictionary of environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/nginx/defaults/main.yml)
