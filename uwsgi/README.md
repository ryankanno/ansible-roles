# uwsgi

This role installs [uwsgi](https://projects.unbit.it/uwsgi/).

## role variables

|name|description|default|
|----|-----------|-------|
|`uwsgi.package`|uwsgi pip package|uwsgi|
|`uwsgi.version`|uwsgi pip package version|2.0.11.1|
|`uwsgi.logs_path`|uwsgi log path|/var/log/uwsgi|
|`uwsgi.apps_conf`|list of uwsgi configuration files||
|`env`|dictionary of environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/uwsgi/defaults/main.yml)
