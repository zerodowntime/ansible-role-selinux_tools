# selinux_tools

nsible role to install selinux auditing tools

## Installation

```yaml
   ansible-galaxy install zerodowntime.selinux_python
   ansible-galaxy install zerodowntime.selinux_tools
```

## Requirements

This role requires Ansible 2.5 or higher.

Supported platforms:

```yaml
  platforms:
    - name: EL
      versions:
        - 7
```

## Default role variables

| Variable name                | Required? |  Type  | Description                           |
|:---------------------------- |:---------:|:------:|:------------------------------------- |
| selinux_tools__package_state |    yes    | string | Key value list of environments to set |

**All variables are described in [defaults/main.yml](defaults/main.yml) file.**

## Static role variables

| Variable name           | Type | Description                                                 |
|:----------------------- |:----:|:----------------------------------------------------------- |
| selinux_tools__packages | list | system packages list names to install selinux selinux_tools |

**All static variables are described in [vars/main.yml](vars/main.yml) file.**

## Example Playbook

```yaml
- hosts: all
  become: true
  roles:

  - role: zerodowntime.selinux_tools
```

## License

[Apache License 2.0](LICENSE)

## Support

ansible@zerodowntime.pl
