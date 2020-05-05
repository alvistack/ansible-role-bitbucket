# Ansible Role for Bitbucket

[![Travis](https://img.shields.io/travis/com/alvistack/ansible-role-bitbucket.svg)](https://travis-ci.com/alvistack/ansible-role-bitbucket)
[![GitHub release](https://img.shields.io/github/release/alvistack/ansible-role-bitbucket.svg)](https://github.com/alvistack/ansible-role-bitbucket)
[![GitHub license](https://img.shields.io/github/license/alvistack/ansible-role-bitbucket.svg)](https://github.com/alvistack/ansible-role-bitbucket/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/galaxy-alvistack.bitbucket-blue.svg)](https://galaxy.ansible.com/alvistack/bitbucket)

Ansible Role for Atlassian Bitbucket Installation.

## Requirements

This role require Ansible 2.9 or higher.

This role was designed for:

  - Ubuntu 18.04/19.10/20.04
  - RHEL/CentOS 7/8
  - openSUSE Leap 15.1
  - Debian 10
  - Fedora 30

## Role Variables

[defaults/main.yml](defaults/main.yml)

## Dependencies

[ansible-role-requirements.yml](ansible-role-requirements.yml)

## Example Playbook

[molecule/default/converge.yml](molecule/default/converge.yml)

This role could simply deploy to `localhost` as below:

    molecule converge -s default

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
