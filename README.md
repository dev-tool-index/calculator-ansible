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
- Execute the playbook

  ```sh
  $ ansible-playbook -i development/hosts site.yml [-v] [--ask-become-pass]
  ```
  
