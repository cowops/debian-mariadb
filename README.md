Debian-Mariadb
==============

An enhanced, drop-in replacement for MySQL.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

mariadb_gpg_key_id: cbcb082a1bb943db
mariadb_series_version: '10.1'

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: loranger.debian-mariadb, mariadb_gpg_key_id: cbcb082a1bb943db, mariadb_series_version: '10.1' }

Tasks
-----

  - Install [MariaDB](https://mariadb.org/en/) server
  - Install [mytop](http://jeremy.zawodny.com/mysql/mytop/)
  

License
-------

BSD