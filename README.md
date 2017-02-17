MariaDB-Server
========

Playbook to install and configure MariaDB-Server on Redhat/Centos,Ubuntu

Requirement
-----------

Redhat/Centos,Ubuntu and Python-setup-tools

Playbook Example
---------------

```

hosts: all
roles:
- mariadb

```

Role Variables
--------------
mariadb/group_vars/all

```

# Installation Variables
# Files to Install on redhat.yml

# Download source for Installing the RPM file for MariaDB-Server
mariadb-server-rpm-file: http://downloads.mariadb.com/MariaDB/mariadb-10.1.21/yum/rhel/mariadb-10.1.21-rhel-7-x86_64-rpms.tar
# Destination var for downloading the file
destination-file: /opt/
#RPM-Key-File
rpm-key: https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
----------
# Files to Install on ubuntu.yml

# mysql-python package 
mysql-python-package: http://mirrors.kernel.org/ubuntu/pool/main/p/python-mysqldb/python3-mysqldb_1.3.7-1build2_amd64.deb
python-mysqldb: /opt/python-mysqldb-dbg_1.3.7-1build2_amd64.deb

#mariadb-client
mariadb-client-package: http://mirrors.kernel.org/ubuntu/pool/universe/m/mariadb-10.0/mariadb-client_10.0.29-0ubuntu0.16.04.1_all.deb
mariadb-client: /opt/mariadb-client_10.0.29-0ubuntu0.16.04.1_all.deb 

#mariadb-server
mariadb-server-package: http://mirrors.kernel.org/ubuntu/pool/universe/m/mariadb-10.0/mariadb-server_10.0.29-0ubuntu0.16.04.1_all.deb
mariadb-server: /opt/mariadb-server_10.0.29-0ubuntu0.16.04.1_all.deb


```
Dependencies
------------
 NONE
 
License
-------
 NONE
 
Author
-----
Nittysh @sainittysh@gmail.com


