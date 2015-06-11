# fail2ban

This role helps configure fail2ban.

By default, only enables ssh/ssh-ddos

## role variables

|name|description|default|
|----|-----------|-------|
|`fail2ban.package`|fail2ban package|fail2ban|
|`fail2ban.version`|fail2ban package version|0.8.11-1|
|`fail2ban.config.src`|fail2ban jail template|jail.local.j2|
|`fail2ban.config.ignoreip`|ip to ignore|127.0.0.1/8|
|`fail2ban.config.bantime`|number of seconds to ban|600|
|`fail2ban.config.banaction`|default banaction|iptables-multiport|
|`fail2ban.config.backend`|default fail2ban backend|auto|
|`fail2ban.config.action`|default action|'%(action_mwl)s'|
|`fail2ban.config.destemail`|email|root@localhost|
|`env`|dictionary of environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/fail2ban/defaults/main.yml)
