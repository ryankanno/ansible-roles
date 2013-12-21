# memcached

This role installs [memcached](http://memcached.org).

## role variables

|name|description|default|
|----|-----------|-------|
|`memcached.package`|memcached package|memcached|
|`memcached.version`|memcached package version|1.4.14-0ubuntu1|
|`memcached.user`|memcached user|memcache|
|`memcached.group`|memcached group|memcache|
|`memcached.config.logfile`|memcached log file|/var/log/memcached.log|
|`memcached.config.memory`|size of cache|64|
|`memcached.config.ip`|ip address to listen on|127.0.0.1|
|`memcached.config.port`|connection port|11211|
|`memcached.config.num_connections`|max simultaneous connections|1024|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/memcached/defaults/main.yml)
