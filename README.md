# popos-ansible


12.10.2021

Some default routines after fresh Pop!_OS 21.04 installation

```bash
# run all playbooks on localhost
ansible-playbook ./playbooks/main.yml --ask-become-pass

# for locales fixing run (popos uses gnome)
gnome-language-selector
```

## todos

```bash
#TODO: set hostname
#TODO: add .gitconfig name + email
#TODO: install snapd + vscode
```