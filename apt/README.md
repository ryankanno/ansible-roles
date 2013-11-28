# apt

This playbook installs and maintains apt.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`apt.cache_valid_time`|seconds between cache updates|3600|
|`apt.should_upgrade`|true if you want to upgrade apt packages|true|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/apt/defaults/main.yml)
