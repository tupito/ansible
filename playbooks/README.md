29.9.2021 
For Pop!_OS 21.04, run locally

```bash
# run all playbooks
ansible-playbook main.yml --ask-become-pass

# for locales fixing run (popos uses gnome)
gnome-language-selector
```