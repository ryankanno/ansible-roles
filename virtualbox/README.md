# virtualbox

This role helps configure the latest guest additions for virtualbox.

## role variables

|name|description|default|
|----|-----------|-------|
|`virtualbox.guest_additions.version`|virtualbox guest additions version|4.3.2|
|`virtualbox.guest_additions.iso_url`|virtualbox guest additions iso download url (depends on version)|http://dlc.sun.com.edgesuite.net/virtualbox/4.3.2/VBoxGuestAdditions_4.3.2.iso|
|`virtualbox.guest_additions.iso_checksum`|virtualbox guest additions iso checksum (depends on version)|f0b8fec99c65231641d5d01558abb53fe8b81f131dc71519cb7994c9e297300d|
|`virtualbox.guest_additions.iso_dir`|virtualbox guest additions iso download directory|/tmp|
|`virtualbox.guest_additions.iso_mountdir`|virtualbox guest additions mount dir|/mnt|
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/virtualbox/defaults/main.yml)
