# ansible-pull
#### Overvew
This project is meant for offline/online configuration management for Linux systems.  Typically clients as they will be internittently connected to the network and are not ideal for centralized ansible management, unlike always on servers.
##### Requirements
The requirements for the client is for ansible to be installed.  Although git is unilized as the central repository for this code, the ansible-pull executable is the only binary needed to kick of this method management.
### Installation
To get started, 
1. Install anible on the client, 
2. Make sure it has Internet access, 
3. Run the following command as root (or sudo):
```bash
ansible-pull -U https://github.com/rscameron42/ansible-pull.git
```
Succsessfully running this job installs an ansible user and a cronjob to check in for changes every 10 minutes
