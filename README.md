Ansible Role: Nginx
=========
[![Build Status](https://travis-ci.org/tenequm/ansible-nginx.svg?branch=master)](https://travis-ci.org/tenequm/ansible-nginx)

This role installs nginx on the server, currently it works only with Ubuntu 16.04 LTS, it's just a skeleton that fits for now and I'm going to make it more flexible and useful with the time of use.

Requirements
------------
This role requires only root access for accomplishing its operations, so either run it in a playbook with a global `become: yes`, or invoke the role in your playbook like:
```
- hosts: localhost
  become: yes
  roles:
    - role: tenequm.nginx
```

Role Variables
--------------

There are no variables for used in there for now, will add them when the role will be more complicated.

Example Playbook
----------------

```
- hosts: localhost
  become: yes
  roles:
    - { role: tenequm.nginx }
```
License
-------

MIT

Author Information
------------------

This role was created in 2017 by [Mykhaylo Kolesnik](http://github.com/tenequm).
