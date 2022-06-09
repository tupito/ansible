# popos-ansible

30.12.2021

Some personal default routines after fresh Pop!_OS 21.04/21.10 installation

## usage 

30.12.2021

```bash
# install ansible
sudo apt install ansible

# clone public repo
git clone https://github.com/tupito/ansible

# run all playbooks on localhost with sudo
ansible-playbook ./playbooks/main.yml --ask-become-pass

# fix locales manually (pop os uses gnome at this point)
gnome-language-selector
```

## todos
### bef 22.04 installation
9.6.2022

* [] var: hostname (stop if null) #TODO
* [] var: email? (gitconfig, aanywhere else?) #TODO
* [] create_ssh_key_only_if_doesnt_exist #TODO
* [] var: ssh key comment #TODO

### maybe someday, notepool
9.6.2022

```
# plugins
* [] browser-plugins (brave, firefox), bitwarden, privacy badger, uBlock origin, I don't care about cookies


* [] hardening: fix umask values, https://www.computernetworkingnotes.com/linux-tutorials/how-to-change-default-umask-permission-in-linux.html
* [] OS settings: settings -> desktop -> background
* [] ssh-copy-id

# packages
* [] install vivaldi, ungoogled chromium, librewolf
* [] install mulvad
* [] unattended-upgrade, security

# misc
* [] restore rsync backups
* [] authorize github access key

# optimization/refactoring:
* [] refactor all apt installs in one module call
* [] refactor all snap installs in one module call
* [] refactor all tasks to "ensure something..." form

# longterm
* [] refactor to ansible role
* [] tests for configurations
* [] solve last modified date issue with git + rsync-backups

```

### not going to fix
* gnome-language-selectro

## dual boot

12.10.2021

https://support.system76.com/articles/bootloader/

https://github.com/spxak1/weywot/blob/main/Pop_OS_Dual_Boot.md

## checklist before new os-installation

30.12.2021

* [] git: all local commits pushed
* [] backups