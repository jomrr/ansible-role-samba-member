# ansible-role-samba-member

![GitHub](https://img.shields.io/github/license/jam82/ansible-role-samba-member) [![Build Status](https://travis-ci.org/jam82/ansible-role-samba-member.svg?branch=main)](https://travis-ci.org/jam82/ansible-role-samba-member)

**Ansible role for setting up Samba as AD Member Server.**

## Supported Platforms

- Alpine
- Archlinux
- CentOS
- Debian
- Fedora
- OpenSuse Leap, Tumbleweed
- OracleLinux
- Ubuntu

## Requirements

Ansible 2.9 or higher.

## Variables

Variables and defaults for this role.

### defaults/main.yml

```yaml
samba_member_role_enabled: false
```

## Dependencies

None.

## Example Playbook

```yaml
---
# role: ansible-role-samba-member
# file: site.yml

- hosts: all
  become: true
  gather_facts: true
  vars:
    samba_member_role_enabled: true
  roles:
    - role: ansible-role-samba-member
```

## License and Author

- Author:: [jam82](https://github.com/jam82/)
- Copyright:: 2021, [jam82](https://github.com/jam82/)

Licensed under [MIT License](https://opensource.org/licenses/MIT).
See [LICENSE](https://github.com/jam82/ansible-role-samba-member/blob/master/LICENSE) file in repository.

## References

- [ArchWiki](https://wiki.archlinux.org/)
