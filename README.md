pcopfer.mariadb
===============

A simple role to install mariadb with some databases.

WARNING
-------

This Role does not implement good security


Role Variables
--------------

- ``mysql_root_password`` Mysql root password
- ``mysql_old_root_password: vault_mysql_password`` Old Mysql root password
- ``mariadb_install_client: false`` Install packages client on system

Example Playbook
----------------


    - hosts: servers
      vars:
         - mysql_databases:
		- db_name: "database1"
		  db_user: "user1"
		  db_password: "Geheim1"
      roles:
         - role: pcopfer.mariadb

License
-------

BSD

Author Information
------------------

pcopfer <christian-platz at pcopfer.de>
