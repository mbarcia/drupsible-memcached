drupsible-memcached
===================

Install and configure Memcached service daemon and its PHP5 memcached extension.

Requirements
------------

This role requires PHP5 FPM (Fast Process Manager) to be present. 
This role can be used indepedently and does NOT require Drupsible to run.

Example Playbook
----------------

```
- role: drupsible.memcached
  when: app_env.memcached|bool
  become: yes
  tags: [ 'role::memcached' ]
```

License
-------

GNU General Public License v3

Author Information
------------------

Mariano Barcia - [https://github.com/mbarcia](https://github.com/mbarcia)
