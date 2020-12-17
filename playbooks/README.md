# localhost playbooks
```bash
# run all playbooks
ansible-playbook main.yml

# testbox, no pwd, more -vvvv == more debug info
ansible-playbook <playbook>.yml -v

# prompts for sudo pwd
ansible-playbook <playbook>.yml --ask-become-pass

# only check
ansible-playbook <playbook>.yml --syntax-check 
```