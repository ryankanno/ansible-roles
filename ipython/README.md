# ipython

This playbook helps configure ipython.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`ipython.package`|ipython package|ipython|
|`ipython.version`|ipython version|0.13.1~rc3-0ubuntu1|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/ipython/defaults/main.yml)

## role dependencies

  * [pythondev](https://github.com/ryankanno/playbooks/blob/master/pythondev)
