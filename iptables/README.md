# iptables

This role installs iptables / iptables-persistent to manage the firewall.

## role variables

|name|description|default|
|----|-----------|-------|
|`iptables.conf.src_path`|path to iptables.j2|iptables.j2|
|`iptables.conf.vars.open_ports`|list of ports to open|22|
|`env`|dictionary of environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/iptables/defaults/main.yml)

## todo

  * Need to update iptables.j2 template
