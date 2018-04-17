
# Vagrant box Ubuntu Xenial64 with postgres 9.4


Ubuntu Xenial64 with postgres 9.4 to play with and do not pollute your computer.


## Prerequisites
- VirtualBox
- Vagrant
- Git

## To Use

Clone the repo

```
$ git clone <repo>
```

Start the VM
```
$ cd <repo>
$ vagrant up
```

Use the box
```
$ vagrant ssh

vagrant-box> psql -U postgres -W -h 127.0.0.1

postgres=# 
```

