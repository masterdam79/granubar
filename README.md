# granubar
open-source self-hosted multi-tenant granular backup and recovery

## Goal
The aim is to provide scripts to create a centralised server using normal linux users to authenticate from which granular backups and recovery can be done.

The backup and recovery scripts will be located in the user space and the user will login to the to be backupped remote server using the users own public key to rdiff full/incremental files and dump any databases.

A web-interface will also provide easy interaction with the scripts and authentication will be done using standard Linux PAM.

## Scope and compatibility
This will be a Linux-only solution and the server scripts will primarly be installable on CentOS 7 being able to connect to any Linux machine with SSH access.

## Dependencies
The scripts will use the following techniques and open source software which the install script will automatically install.
* Linux
* Apache
* MySQL
* PHP
* rdiff
* rsync
* mysqldump
* tar
* gzip

## Targets
* The project will seek compatibility with ReaR (https://github.com/rear/rear) for disaster recovery but methods are of this moment unsure.
