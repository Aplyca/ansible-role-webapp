# Ansible Role: WebApp

[![Build Status](https://travis-ci.org/Aplyca/ansible-role-webapp.svg?branch=master)](https://travis-ci.org/Aplyca/ansible-role-webapp)

Ansible Role that installs an configure a WebApp (website) on Debian/Ubuntu.

## Requirements

Use hash behavior for variables in ansible.cfg
See example: https://github.com/Aplyca/ansible-role-apache/blob/master/tests/ansible.cfg
See official docs: http://docs.ansible.com/intro_configuration.html#hash-behaviour

## Installation

Using ansible galaxy:
```bash
ansible-galaxy install mauricios.WebApp
```
You can add this role as a dependency for other roles, add the role to the meta/main.yml file of your own role:
```yaml
dependencies:
  - { role: mauricios.WebApp }
```

## Role Variables

See default variables: https://github.com/Aplyca/ansible-role-webapp/blob/master/defaults/main.yml

## Dependencies

Install dependencies using Ansible galaxy

`ansible-galaxy install -r dependencies.txt`

## Testing

Use Vagrant to test the role:

```bash
cd tests;
vagrant box add ubuntu/trusty64;
vagrant up;
```
You should see your WebApp runnig on http://webapp.com:8080

## License

MIT / BSD

## Author Information

Mauricio Sánchez from Aplyca SAS (http://www.aplyca.com)
