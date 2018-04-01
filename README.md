Debian-Mariadb
==============

An enhanced, drop-in replacement for MySQL.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

debian:
    version: stretch
mariadb:
    gpg_key_id: F1656F24C74CD1D8
    series_version: '10.2'
    mirror: ftp.igh.cnrs.fr/pub

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-mariadb, debian.version: stretch, mariadb.gpg_key_id: F1656F24C74CD1D8, mariadb.series_version: '10.2', mariadb.mirror: 'ftp.igh.cnrs.fr/pub' }

Tasks
-----

  - Install [MariaDB](https://mariadb.org/en/) server
  - Install [mytop](http://jeremy.zawodny.com/mysql/mytop/)


License
-------

BSD
