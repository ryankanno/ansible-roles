# ntp

This playbook installs ntp.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`ntp.servers`|list of ntp servers|0.pool.ntp.org, 1.pool.ntp.org, 2.pool.ntp.org, 3.pool.ntp.org|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/ntp/defaults/main.yml)
