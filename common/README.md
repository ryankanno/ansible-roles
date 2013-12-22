# common

This role installs a common set of libraries / packages and configures a 
more secure installation.

## role variables

|name|description|default|
|----|-----------|-------|
|`common.users.to_remove`|list of users to remove|games, irc, list, news, proxy, uucp|
|`common.groups.to_remove`|list of groups to remove|games, irc, list, news, proxy, uucp|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/common/defaults/main.yml)

## role dependencies

  * [apt](https://github.com/ryankanno/ansible-roles/blob/master/apt)
  * [sslcerts](https://github.com/ryankanno/ansible-roles/blob/master/sslcerts)
  * [timezone](https://github.com/ryankanno/ansible-roles/blob/master/timezone)
  * [ntp](https://github.com/ryankanno/ansible-roles/blob/master/ntp)
  * [hostname](https://github.com/ryankanno/ansible-roles/blob/master/hostname)
  * [sshd](https://github.com/ryankanno/ansible-roles/blob/master/sshd)
  * [iptables](https://github.com/ryankanno/ansible-roles/blob/master/iptables)
  * [fail2ban](https://github.com/ryankanno/ansible-roles/blob/master/fail2ban)
