# shhirose.keymap

[![Github](https://img.shields.io/badge/github-shhirose%2Fansible--keymap-brightgreen.svg)](https://github.com/shhirose/ansible-keymap)
[![Ansible galaxy](https://img.shields.io/badge/ansible--galaxy-keymap-brightgreen.svg)](https://galaxy.ansible.com/shhirose/keymap/)
[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)

This is Ansible role for keyboard setting for RedHat Enterprise Linux.

## Requirements

None

## Role Variables

```
shhirose_keymap_keytable: "us"
shhirose_keymap_model: "PC105+inet"
shhirose_keymap_layout: "us"
shhirose_keymap_keyboardtype: "pc"
```

## Variable parameters

| key | required | default | type | values | notes |
| --- | --- | --- | --- | --- | --- |
| shhirose_keymap_keytable | no |  | string | jp106 |  |
| shhirose_keymap_model | no |  | string | jp106 |  |
| shhirose_keymap_layout | no |  | string | jp |  |
| shhirose_keymap_keyboardtype | no |  | string | pc |  |

## Dependencies

None

## Example Playbook

```
- hosts: servers
  become: yes
  roles:
    - shhirose.keymap
  vars:
    shhirose_keymap_keytable: 'jp106'
    shhirose_keymap_model: 'jp106'
    shhirose_keymap_layout: 'jp'
```

## License

MIT
