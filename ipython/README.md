# ipython

This playbook helps configure ipython

## playbook variables

|name|description|default|
|----|-----------|-------|
|`ipython.version`|ipython version|0.13.1~rc3-0ubuntu1|
|`env.proxies`|dictionary of environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/ipython/defaults/main.yml)

## role dependencies

  * [common](https://github.com/ryankanno/playbooks/blob/master/common)
  * [pythondev](https://github.com/ryankanno/playbooks/blob/master/pythondev)
