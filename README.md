# popos-ansible

Some personal default routines after fresh Pop!_OS 22.04 installation

## edit ./run-localhost.yml before running
16.8.2024

uncomment wanted roles and setup:

* hostname
* gitconfig
* ssh-key

## run

```bash
# install ansible
sudo apt install ansible
# clone public repo
git clone https://github.com/tupito/ansible
# run roles for localhost
./run-localhost.sh
```

## TODO

```bash
/etc/apt/apt.conf.d/99nocache
  APT::Keep-Downloaded-Packages "false";
```