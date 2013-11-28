# logrotate

This playbook helps configure logrotate.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`logrotate.package`|logrotate package|logrotate|
|`logrotate.version`|logrotate package version|3.7.8-6ubuntu6|
|`logrotate.config.rotation_schedule`|log rotation schedule|weekly|
|`logrotate.config.num_rotate`|number of weeks worth of logs to keep|4|
|`logrotate.config.should_compress`|compress logs?|true|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/logrotate/defaults/main.yml)
