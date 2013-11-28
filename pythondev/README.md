# pythondev

This playbook installs packages / libraries associated with python development.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`python.package`|python package|python2.7|
|`python.version`|python package version|2.7.3-5ubuntu4|
|`python.libraries.latest`|latest python packages to install|python-dev, python-pip, python-virtualenv|
|`python.libraries.versioned`|versioned python packages to install||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/pythondev/defaults/main.yml)
