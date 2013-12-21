# sudo

This playbook helps configure sudo access for a user.

*Note*: This gives passwordless, root privileges to the users defined.

## playbook variables

|name|description|default|
|----|-----------|-------|
|`sudo.users`|list of users to give sudo to||

|name|description|value type|
|----|-----------|-------|
|`user.name`|user to create||
|`user.is_system`|is user a system account|1 or 0|
|`user.should_create_home`|should user home be created|1 or 0|
|`user.should_generate_ssh_key`|should user ssh keys be generated|1 or 0|


See [defaults/main.yml](https://github.com/ryankanno/playbooks/blob/master/sudo/defaults/main.yml)
