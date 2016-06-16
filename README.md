drupsible-memcached
===================

Install and configure Memcached service daemon. If PHP-FPM is present in the system, also install the PHP memcached extension.

Requirements
------------

This role DOES NOT requires PHP-FPM (Fast Process Manager) to be present. But if it is, it will install the PHP memcached extension (both PHP5 and PHP7 are supported).

This role can be used indepedently and does NOT require Drupsible to run.

Example Playbook
----------------

```
- role: drupsible.memcached
  when: app_memcached_enabled|default(True)|bool
  become: yes
  tags: [ 'role::memcached' ]
```

License
-------

GNU General Public License v3

Author Information
------------------

Mariano Barcia - [https://github.com/mbarcia](https://github.com/mbarcia)
