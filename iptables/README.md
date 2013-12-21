# iptables

This role installs iptables / iptables-persistent to manage the firewall.

## role variables

|name|description|default|
|----|-----------|-------|
|`iptables.open_ports`|list of ports to open|22|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/iptables/defaults/main.yml)
