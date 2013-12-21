# varnish

This role installs [varnish](http://varnish-cache.org).

## role variables

|name|description|default|
|----|-----------|-------|
|`varnish.package`|varnish package|varnish|
|`varnish.version`|varnish package version|3.0.2-2|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/varnish/defaults/main.yml)
