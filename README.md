git Ansible role: virtualbox
=========

This role helps you to install virtualbox on your linux machine.


|Travis|CircleCI|GitHub|Quality|Downloads|Version|
|------|--------|------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-virtualbox.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-virtualbox)|![circleci](https://circleci.com/gh/amine7777/ansible-role-virtualbox.svg?style=svg)|[![github](https://github.com/amine7777/ansible-role-virtualbox/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-virtualbox/actions)|[![quality](https://img.shields.io/ansible/quality/50498)](https://galaxy.ansible.com/amine7777/virtualbox)|[![downloads](https://img.shields.io/ansible/role/d/50348)](https://galaxy.ansible.com/amine7777/virtualbox)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-virtualbox.svg)](https://github.com/amine7777/ansible-role-virtualbox/releases/)|

![](virtualbox.jpg)

Requirements
------------
- Linux machine
- Ansible 2.9

Role Variables
--------------
These variables helps to manage virtualbox installation.

You can specify your virtualbox version in this variable.
```yaml
virtualbox_version: 0.13.1
virtualbox_arch: amd64
virtualbox_directory_path: /usr/local/bin
```
This is the url where virtualbox will be downloaded.
```yaml
virtualbox_download_url: 'https://releases.hashicorp.com/virtualbox/{{ virtualbox_version }}/virtualbox_{{ virtualbox_version }}_linux_{{ virtualbox_arch }}.zip'
```
This is the path where packer binary will be stored.
```yaml
virtualbox_directory_path: /usr/local/bin
```

Example Playbook
----------------

```yaml
- hosts: all
  roles:
     - amine7777.virtualbox
```


Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
