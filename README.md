# granubar
open-source self-hosted multi-tenant granular backup and recovery

## Goal
The aim is to provide scripts to create a centralised server using normal linux users to authenticate from which granular backups and recovery can be done.

The backup and recovery scripts will be located in the user space and the user will login to the to be backupped remote server using the users own public key to rdiff full/incremental files and dump any databases.

A web-interface will also provide easy interaction with the scripts and authentication will be done using standard Linux PAM.

# Scope
This will be a Linux-only solution

## Targets
* The project will seek compatibility with ReaR for disaster recovery.