# supervisor

This role installs [supervisor](http://supervisord.org/).

## role variables

|name|description|default|
|----|-----------|-------|
|`supervisor.package`|supervisor pip package|supervisor|
|`supervisor.version`|supervisor pip package version|3.0b2|
|`supervisor.conf.src_path`|supervisor config path|supervisord.conf.j2|
|`supervisor.logs_path`|supervisor child log path|/var/log/supervisord|
|`supervisor.apps_conf`|list of supervisor configuration files||
|`env`|dictionary of environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/supervisor/defaults/main.yml)
