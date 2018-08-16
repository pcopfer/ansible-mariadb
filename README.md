pcopfer.mariadb
===============

A simple role to install mariadb with some databases.

WARNING
-------

This Role does not implement good security


Role Variables
--------------

- ``mariadb_bind_address: "127.0.0.1"`` Address mariadb listen to connections
- ``ufw_mariadb_public: false`` Allow connections to mariadb in ufw
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
