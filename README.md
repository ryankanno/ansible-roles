# Ansible-Roles

## Here be dragons

My tiny collection of [Ansible](https://github.com/ansible/ansible) roles.

Follow the instructions over at [vagrant-ansible](https://github.com/ryankanno/vagrant-ansible) to play around with them!

## Updates

  * Added env.proxies as an environment variable for all tested roles
  * Updated README in each role describing all the available variables
  * Tried to make each task idempotent (If you see anything that stinks, I take pull requests!)

## Roles

### Tested

  * [apt](https://github.com/ryankanno/ansible-roles/tree/master/apt)
  * [common](https://github.com/ryankanno/ansible-roles/tree/master/common)
  * [fail2ban](https://github.com/ryankanno/ansible-roles/tree/master/fail2ban)
  * [haproxy](https://github.com/ryankanno/ansible-roles/tree/master/haproxy)
  * [hostname](https://github.com/ryankanno/ansible-roles/tree/master/hostname)
  * [iptables](https://github.com/ryankanno/ansible-roles/tree/master/iptables)
  * [ipython](https://github.com/ryankanno/ansible-roles/tree/master/ipython)
  * [ipython-notebook](https://github.com/ryankanno/ansible-roles/tree/master/ipython-notebook)
  * [javadev](https://github.com/ryankanno/ansible-roles/tree/master/javadev)
  * [javaenv](https://github.com/ryankanno/ansible-roles/tree/master/javaenv)
  * [logrotate](https://github.com/ryankanno/ansible-roles/tree/master/logrotate)
  * [lynis](https://github.com/ryankanno/ansible-roles/tree/master/lynis)
  * [memcached](https://github.com/ryankanno/ansible-roles/tree/master/memcached)
  * [motd](https://github.com/ryankanno/ansible-roles/tree/master/motd)
  * [ntp](https://github.com/ryankanno/ansible-roles/tree/master/ntp)
  * [pythondev](https://github.com/ryankanno/ansible-roles/tree/master/pythondev)
  * [redis](https://github.com/ryankanno/ansible-roles/tree/master/redis)
  * [rubydev](https://github.com/ryankanno/ansible-roles/tree/master/rubydev)
  * [rvm](https://github.com/ryankanno/ansible-roles/tree/master/rvm)
  * [sshd](https://github.com/ryankanno/ansible-roles/tree/master/sshd)
  * [sslcerts](https://github.com/ryankanno/ansible-roles/tree/master/sslcerts)
  * [sudo](https://github.com/ryankanno/ansible-roles/tree/master/sudo)
  * [timezone](https://github.com/ryankanno/ansible-roles/tree/master/timezone)
  * [virtualbox](https://github.com/ryankanno/ansible-roles/tree/master/virtualbox)

### Dragons

  * [elasticsearch](https://github.com/ryankanno/ansible-roles/tree/master/elasticsearch)
  * [logstash](https://github.com/ryankanno/ansible-roles/tree/master/logstash)
  * [monit](https://github.com/ryankanno/ansible-roles/tree/master/monit)
  * [nginx](https://github.com/ryankanno/ansible-roles/tree/master/nginx)
  * [rsyslog](https://github.com/ryankanno/ansible-roles/tree/master/rsyslog)
  * [sysctl](https://github.com/ryankanno/ansible-roles/tree/master/sysctl)
  * [uwsgi](https://github.com/ryankanno/ansible-roles/tree/master/uwsgi)
  * [varnish](https://github.com/ryankanno/ansible-roles/tree/master/varnish)

### TODO (Needs to be migrated)

  * kibana
  * hadoop
  * openvpn
  * hadoop
  * jenkins
  * mysql
  * postgres
  * kafka
  * sonarqube
  * sonarqube-runner
  * storm

## Tips

  * If you get apt install errors related to being unable to find a version, please add
    the apt role. Most of the default package variables are up to date so they
    require an updated apt cache.  I generally don't include update_cache in individual 
    apt module calls - just to keep things simple. I also removed the apt meta 
    dependency to make things more explicit.
