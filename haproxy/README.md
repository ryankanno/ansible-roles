# haproxy

This role installs and configures [haproxy](http://haproxy.1wt.eu/).

## details

  * Installs logrotate config

## role variables

|name|description|default|
|----|-----------|-------|
|`haproxy.package`|haproxy package|haproxy|
|`haproxy.version`|haproxy package version|1.4.18-0ubuntu2|
|`haproxy.user`|haproxy user|haproxy|
|`haproxy.group`|haproxy group|haproxy|
|`haproxy.config.global.maxconn`|max number of global conn|4096|
|`haproxy.config.defaults`|haproxy default config|
      log     global
      mode    http
      option  httplog
      option  dontlognull
      option  redispatch
      retries 3
      maxconn 2000
      contimeout 5000
      clitimeout 50000
      srvtimeout 50000|
|`haproxy.config.applications`|haproxy application specific config|
        listen  web 0.0.0.0:10000
        option  httpchk GET /check.html
        balance roundrobin
        server  web1 web1:80 check inter 2000 fall 3
        server  web2 web2:80 check inter 2000 fall 3|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/haproxy/defaults/main.yml)

## role dependencies

  * [logrotate](https://github.com/ryankanno/ansible-roles/blob/master/logrotate)
