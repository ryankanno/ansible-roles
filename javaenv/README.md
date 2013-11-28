# javaenv

This playbook installs packages / libraries associated with a java environment.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`java.jre.package`|java jre package|openjdk-7-jre|
|`java.jre.version`|java jre package version|7u25-2.3.10-1ubuntu0.12.10.2|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/javaenv/defaults/main.yml)
