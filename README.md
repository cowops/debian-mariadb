Debian-Mariadb
==============

An enhanced, drop-in replacement for MySQL.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

debian:
    version: wheezy
mariadb:
    gpg_key_id: cbcb082a1bb943db
    series_version: '10.1'
    mirror: ftp.igh.cnrs.fr/pub

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-mariadb, debian.version: wheezy, mariadb.gpg_key_id: cbcb082a1bb943db, mariadb.series_version: '10.1', mariadb.mirror: 'ftp.igh.cnrs.fr/pub' }

Tasks
-----

  - Install [MariaDB](https://mariadb.org/en/) server
  - Install [mytop](http://jeremy.zawodny.com/mysql/mytop/)


License
-------

BSD
