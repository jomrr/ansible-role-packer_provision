# ansible-role-packer-provision

Ansible role for use with [packer](https://packer.io) provisioner [ansible](https://www.packer.io/docs/provisioners/ansible.html).

## Supported Platforms

* Archlinux
* CentOs 8
* Ubuntu 18.04

## Requirements

Ansible 2.7 or higher is recommended.

## Variables

Variables and defaults for this role:

| variable | default value in defaults/main.yml | description |
| -------- | ---------------------------------- | ----------- |
| packer_builder_type | 'virtualbox-iso' | emulates packer variable for molecule default test, see [docs](https://www.packer.io/docs/provisioners/ansible.html#default-extra-variables) |
| packer_provision_vagrant | False | Includes the tasks for building public vagrant boxes when True |

## Dependencies

None.

## Example Playbook

```yaml
---
# role: ansible-role-packer-provision
# file: provision.yml

- hosts: packer_provision_systems
  become: True
  roles:
    - role: ansible-role-packer-provision
```

## License and Author

* Author:: Jonas Mauer (<jam@kabelmail.net>)
* Copyright:: 2019, Jonas Mauer

Licensed under MIT License;
See LICENSE file in repository.

## References

* [Packer.io Docs](https://www.packer.io/docs/)
