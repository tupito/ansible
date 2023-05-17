# popos-ansible

17.5.2023

Some personal default routines after fresh Pop!_OS 22.04 installation

required custom vars:
* my_hostname

refactoring from old-playbooks to roles ongoing...

## usage 

17.5.2023

```bash
# install ansible
sudo apt install ansible
# clone public repo
git clone https://github.com/tupito/ansible
# run roles for localhost
./run-localhost.sh

```

## possible todos
9.6.2022


* [] browser-plugins (brave, firefox), bitwarden, privacy badger, uBlock origin, I don't care about cookies
* [] hardening: fix umask values, https://www.computernetworkingnotes.com/linux-tutorials/how-to-change-default-umask-permission-in-linux.html
* [] OS settings: settings -> desktop -> background
* [] ssh-copy-id

### packages
* [] install vivaldi, ungoogled chromium, librewolf
* [] install mulvad
* [] unattended-upgrade, security

### misc
* [] restore rsync backups
* [] authorize github access key

### optimization/refactoring:
* [] refactor all apt installs in one module call
* [] refactor all snap installs in one module call
* [] refactor all tasks to "ensure something..." form

### longterm
* [] tests for configurations
* [] solve last modified date issue with git + rsync-backups