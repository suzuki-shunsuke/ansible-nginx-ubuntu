nginx-ubuntu
==============

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-nginx-ubuntu.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-nginx-ubuntu)

Install Nginx on Ubuntu.

https://galaxy.ansible.com/suzuki-shunsuke/nginx-ubuntu/

Requirements
------------

Nothing.

Role Variables
--------------

* nginx_use_ppa: Whether use ppa to install nginx or not. The default value is "no".
* nginx_upgrade: Whether upgrade nginx if it has already installed. The default value is "no".
* nginx_nonroot: Whether the remote_user is root or not. This variable is set automatically, and is used to execute tasks with the become option.

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - role: suzuki-shunsuke.nginx-ubuntu
    nginx_use_ppa: yes
    nginx_upgrade: no
```

License
-------

MIT
