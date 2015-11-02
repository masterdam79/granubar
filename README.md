# Granubar
open-source self-hosted multi-tenant **Gr**(a)**nu**(lar) **ba**(ckup and )**r**(ecovery).

## Goal
The aim is to provide scripts to create a centralised server using normal linux users from which granular backups and recovery can be done.

The backup and recovery scripts will be located on the to be backupped remote server and write the data to the backup server's user home configured for this client.

A web-interface will also provide easy interaction with the scripts and authentication will be done using standard Linux PAM.
As the backup clients will connect to the backup server and not the other way around, the webinterface will only function to check the consistency of the backups.

## Scope and compatibility
This will be a Linux-only solution and the server scripts will primarly be installable on CentOS 7 being able to connect to any Linux machine with SSH access.

## Dependencies
The scripts will use the following techniques and open source software which the installer will automatically install where applicable.
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

## Security
The security should of course be tight, the back-up clients will connect to the backup server's normal user accounts and write to these user homes.

## Encryption
Files should be encrypted before transmit to the backup server.

# Todo
* Think about the setup
* Think about the security
* Think about the encryption
