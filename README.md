# Playbooks

## Here be dragons

My [Ansible](https://github.com/ansible/ansible) playbooks.

As a warning, these playbooks will be in somewhat a state of flux for the next
few weeks as I migrate infrastructure codes to Ansible.  These are generally
the technologies I tend to install for new machines.

Follow the instructions over at [vagrant-ansible](https://github.com/ryankanno/vagrant-ansible) to play around with them!

## Updates

  * Added env.proxies as an environment variable for all tested playbooks
  * Updated README in each playbook describing all the available variables
  * Tried to make each task idempotent (If you see anything that stinks, I take pull requests!)

## Playbooks

### Tested

  * [apt](https://github.com/ryankanno/playbooks/tree/master/apt)
  * [fail2ban](https://github.com/ryankanno/playbooks/tree/master/fail2ban)
  * [hostname](https://github.com/ryankanno/playbooks/tree/master/hostname)
  * [iptables](https://github.com/ryankanno/playbooks/tree/master/iptables)
  * [ipython](https://github.com/ryankanno/playbooks/tree/master/ipython)
  * [ipython-notebook](https://github.com/ryankanno/playbooks/tree/master/ipython-notebook)
  * [javadev](https://github.com/ryankanno/playbooks/tree/master/javadev)
  * [javaenv](https://github.com/ryankanno/playbooks/tree/master/javaenv)
  * [logrotate](https://github.com/ryankanno/playbooks/tree/master/logrotate)
  * [memcached](https://github.com/ryankanno/playbooks/tree/master/memcached)
  * [motd](https://github.com/ryankanno/playbooks/tree/master/motd)
  * [ntp](https://github.com/ryankanno/playbooks/tree/master/ntp)
  * [pythondev](https://github.com/ryankanno/playbooks/tree/master/pythondev)
  * [redis](https://github.com/ryankanno/playbooks/tree/master/redis)
  * [rubydev](https://github.com/ryankanno/playbooks/tree/master/rubydev)
  * [rvm](https://github.com/ryankanno/playbooks/tree/master/rvm)
  * [sshd](https://github.com/ryankanno/playbooks/tree/master/sshd)
  * [sslcerts](https://github.com/ryankanno/playbooks/tree/master/sslcerts)
  * [timezone](https://github.com/ryankanno/playbooks/tree/master/timezone)
  * [virtualbox](https://github.com/ryankanno/playbooks/tree/master/virtualbox)

### Dragons

  * [elasticsearch](https://github.com/ryankanno/playbooks/tree/master/elasticsearch)
  * [haproxy](https://github.com/ryankanno/playbooks/tree/master/haproxy)
  * [logstash](https://github.com/ryankanno/playbooks/tree/master/logstash)
  * [nginx](https://github.com/ryankanno/playbooks/tree/master/nginx)
  * [rsyslog](https://github.com/ryankanno/playbooks/tree/master/rsyslog)
  * [uwsgi](https://github.com/ryankanno/playbooks/tree/master/uwsgi)
  * [varnish](https://github.com/ryankanno/playbooks/tree/master/varnish)

### TODO (Needs to be migrated)

  * kibana
  * hadoop
  * openvpn
  * hadoop
  * mysql
  * monit
  * postgres
  * kafka
  * storm

## Tips

  * If you get apt install errors related to being unable to find a version, please add
    the apt role. Most of the default package variables are up to date so they
    require an updated apt cache.  I generally don't include update_cache in individual 
    apt module calls - just to keep things simple. I also removed the apt meta 
    dependency to make things more explcit and being able to just call it once for the entire playbook.
