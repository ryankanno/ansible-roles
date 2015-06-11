# sshd

This role helps configure sshd.

## role variables

|name|description|default|
|----|-----------|-------|
|`sshd.package`|sshd package|openssh-server|
|`sshd.version`|sshd package version|1:6.6p1-2ubuntu2|
|`sshd.config.src`|sshd config template|ssh_config.j2|
|`sshd.config.port`|sshd port|22|
|`sshd.config.enable_pam_auth`|enable pam|no|
|`sshd.config.enable_password_auth`|enable password auth|no|
|`sshd.config.enable_pub_key_auth`|enable public key auth|yes|
|`env`|dictionary of environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/sshd/defaults/main.yml)
