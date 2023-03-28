Debian-Mariadb
==============

An enhanced, drop-in replacement for MySQL.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

mariadb:
    series_version: '10.5'
    mirror: ftp.igh.cnrs.fr/pub

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-mariadb, mariadb.series_version: '10.5', mariadb.mirror: 'ftp.igh.cnrs.fr/pub' }

Tasks
-----

  - Install [MariaDB](https://mariadb.org/en/) server
  - Install [mytop](http://jeremy.zawodny.com/mysql/mytop/)


License
-------

BSD
