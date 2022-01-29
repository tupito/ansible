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

30.12.2021

```bash
# OS-installation:
## TODO: [] fix umask values, https://www.computernetworkingnotes.com/linux-tutorials/how-to-change-default-umask-permission-in-linux.html
## TODO: [] Repair boot-boader, check dualboot links
## TODO: [] OS settings: settings -> desktop -> general -> show maximize button
## TODO: [] OS settings: settings -> desktop -> dock -> dock size small
## TODO: [] OS settings: settings -> desktop -> dock -> intelligently hide
## TODO: [] OS settings: settings -> desktop -> background

## TODO: [] ssh-copy-id

# packages
## TODO: [] install sshfs
## TODO: [] install vivaldi
## TODO: [] install mulvad
## TODO: [] install vlc (apt)

# plugins
## TODO: [] browser-plugins (brave, firefox)

# misc
## TODO: [] restore rsync backups
## TODO: [] authorize github access key

# optimization/refactoring:
## TODO: [] refactor all apt installs in one module call
## TODO: [] refactor all snap installs in one module call
## TODO: [] refactor all tasks to "ensure something..." form

# longterm
## TODO: [] refactor to ansible role
## TODO: [] vars: hostname, ssh-key comment, gitconfig, create_ssh_key_only_if_doesnt_exist
## TODO: [] tests for configurations
## TODO: [] solve last modified date issue with git + rsync-backups

# NOT GOING TO FIX:
## gnome-language-selector
```

## dual boot

12.10.2021

https://support.system76.com/articles/bootloader/

https://github.com/spxak1/weywot/blob/main/Pop_OS_Dual_Boot.md

## checklist before new os-installation

30.12.2021

* [] git: all local commits pushed
* [] backups