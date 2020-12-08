# vagrants

Two single vagrantfiles for isolated localhost testing

## common vagrant cmds

```bash
# create default Vagrantfile template with single machine
vagrant init ubuntu/focal64
vagrant init centos/8

# in Vagrantfile directory
vagrant status
vagrant up          # all
vagrant up <boxname>
vagrant ssh <boxname>       
vagrant destroy -f
```

## centos8 + ansible: create and start
```bash
vagrant destroy -f && \
rm -f Vagrantfile && \
vagrant init && \
cp Vagrantfile Vagrantfile.default && \
cp Vagrantfile.centos Vagrantfile && \
vagrant up
```

## ubuntu20.04 + ansible:  create and start
```bash
vagrant destroy -f && \
rm -f Vagrantfile && \
vagrant init && \ 
cp Vagrantfile Vagrantfile.default && \
cp Vagrantfile.ubuntu Vagrantfile && \
vagrant up
```