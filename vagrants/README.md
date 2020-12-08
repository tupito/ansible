```bash
# create default Vagrantfile with sigle machine
vagrant init ubuntu/focal64
vagrant init centos/8

# in Vagrantfile directory
vagrant status

vagrant up          # all
vagrant up <boxname>

vagrant ssh <boxname>       
vagrant destroy -f
```