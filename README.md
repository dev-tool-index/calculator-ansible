# calculator-ansible
[![Build Status](https://travis-ci.org/dev-tool-index/calculator-ansible.svg?branch=master)](https://travis-ci.org/dev-tool-index/calculator-ansible)

## Prerequisites

- [Ansible](https://www.ansible.com/)

  ```sh
  $ ansible --version
  ansible 2.2.1.0
  ```

- [Passwordless SSH Logons on localhost](http://www.serverlab.ca/tutorials/linux/administration-linux/passwordless-ssh-logons-on-centos-6-using-rsa-authentication-keys/)
  

## Run
- Start a centos docker container as dev env.

  ```sh
  $ docker run --add-host=some_docker_container:127.0.0.1 --privileged -it -e "container=docker"  -v /sys/fs/cgroup:/sys/fs/cgroup -p 80:80 --name mycentos -d centos:7 /usr/sbin/init
  ```

- Execute the playbook

  ```sh
  $ ansible-playbook -i development/hosts site.yml [-v] [--ask-become-pass]
  ```
  
