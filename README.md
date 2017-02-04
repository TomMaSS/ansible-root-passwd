ansible-root-passwd
===================

This role chage root password

[![Ansible Galaxy](https://img.shields.io/ansible/role/xxxx.svg)](https://galaxy.ansible.com/salamachinas/root-pswd/)

Requirements
------------

This role requires Ansible 2.0 or higher and platform requirements are listed
in the metadata file.

Install
-------

```sh
ansible-galaxy install salamachinas.root-passwd
```

Hash password
-------------

```sh
openssl passwd -1 -salt xyz  s3cr3t
```

Tests
-----

```sh
docker build -t test-ansible-root-passwd-centos7 -f tests/Dockerfile_centos7 --force-rm .
docker build -t test-ansible-root-passwd-debian7 -f tests/Dockerfile_debian7 --force-rm .
docker build -t test-ansible-root-passwd-debian8 -f tests/Dockerfile_debian8 --force-rm .
docker build -t test-ansible-root-passwd-ubuntu14 -f tests/Dockerfile_ubuntu14 --force-rm .
docker build -t test-ansible-root-passwd-ubuntu16 -f tests/Dockerfile_ubuntu16 --force-rm .
```
