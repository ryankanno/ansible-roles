# ipython-notebook

This role helps configure a secure [ipython-notebook](http://ipython.org/notebook.html).

  * Creates a cert for https
  * Creates a password for the notebook

Log into the box and start the notebook with the following:

`ipython notebook --profile=vagrant`

## role variables

|name|description|default|
|----|-----------|-------|
|`ipython_notebook.package`|ipython-notebook package|ipython-notebook|
|`ipython_notebook.version`|ipython version|0.13.1~rc3-0ubuntu1|
|`ipython_notebook.scientific_libraries`|ipython scientific libraries|python-matplotlib, python-scipy, python-pandas, python-nose|
|`ipython_notebook.default_notebook_password`|ipython notebook password if you don't pass the sha1 password|bar|
|`ipython_notebook.notebooks`|list of notebooks to configure (see below)||
|`env.proxies`|dictionary of proxy related environment variables (http_proxy, https_proxy, ftp_proxy)||

### notebook config variables
|name|description|default|
|----|-----------|-------|
|`user`|user who owns the notebook|vagrant|
|`group`|group who owns the notebook|vagrant|
|`config.ip`|ip address the notebook is being served on|* (all interfaces)|
|`config.port`|port the notebook is listening on|9999|
|`config.profile`|name of the notebook profile|vagrant|
|`config.sha1_password`|notebook password||
|`config.certfile`|certfile to use for notebook (if defined, the options below are ignored)||
|`config.certfile_subject`|cert subject|/C=US/ST=HI/L=Honolulu/O=IT/CN={{ ansible_fqdn }}|
|`config.certfile_dir`|directory to save generated cert|/home/vagrant/ssl/cert|
|`config.notebook_dir`|directory to store the notebook files|/home/vagrant/notebooks|


See [defaults/main.yml](https://github.com/ryankanno/ansible-roles/blob/master/ipython-notebook/defaults/main.yml)

## role dependencies

  * [ipython](https://github.com/ryankanno/ansible-roles/blob/master/ipython)
