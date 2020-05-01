# ansible-role-packer-provision

**Ansible role for use with [packer](https://packer.io) provisioner [ansible](https://www.packer.io/docs/provisioners/ansible.html).**

## Supported Platforms

- Alpine 3.11
- Archlinux
- CentOS 8
- Debian 9, 10
- Fedora 31
- Ubuntu 18.04, 20.04

## Requirements

Ansible 2.9 or higher is recommended.

## Variables

| variable | default value in defaults/main.yml | description |
| -------- | ---------------------------------- | ----------- |
| packer_builder_type | 'virtualbox-iso' | packer internal variable for builder type, see [docs](https://www.packer.io/docs/provisioners/ansible.html#default-extra-variables) |

## Dependencies

None.

## License and Author

- Author:: [jam82](https://github.com/jam82/)
- Copyright:: 2020, [jam82](https://github.com/jam82/)

Licensed under [MIT License](https://opensource.org/licenses/MIT).
See [LICENSE](https://github.com/jam82/ansible-role-packer-provision/blob/master/LICENSE) file in repository.

## References

- [Packer.io Docs](https://www.packer.io/docs/)
