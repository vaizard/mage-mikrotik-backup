# mage-mikrotik-backup
Ansible role to deploy a script that generates and pulls mikrotik backups over ssh and stores them in a git repo. This role configures

- the openssh client by putting the /etc/ssh/config.d/mikrotik-backup file (NOTE that this assumes that the ssh config file contains the propper Include directive (this is configured i.e. by the https://github.com/vaizard/mage-openssh role, so if you manage openssh differently, configure your roles accordingly)
- a host list and a cronjob that runs the backup-pull script.


