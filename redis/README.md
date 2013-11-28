# redis

This playbook installs [redis](http://redis.io).

## playbook variables

|name|description|default|
|----|-----------|-------|
|`redis.package`|redis package|redis-server|
|`redis.version`|redis package version|2:2.4.15-1|
|`redis.config_dir`|redis config dir|/etc/redis|
|`redis.user`|redis user|redis|
|`redis.group`|redis group|redis|
|`redis.config.num_databaseses`|number of databases|16|
|`redis.config.password`|redis password|64|
|`redis.config.pid_file`|pid_file|/var/run/redis.pid|
|`redis.config.port`|connection port|6379|
|`redis.config.working_dir`|working directory|/var/db/redis|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/redis/defaults/main.yml)
