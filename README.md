# ansible-role-ddev

A role for [Ansible](https://github.com/ansible/ansible), that installs [DDEV](https://ddev.readthedocs.io/en/stable) for launching local PHP development environments.

## Requirements

The only requirements needed for this role is [ansible-role-docker](https://github.com/geerlingguy/ansible-role-docker) from [geerlingguy](https://github.com/geerlingguy), which is built into this role.

## Quick start

1. First clone this repository and add into your project directory.
2. Include the role in your [Ansible](https://github.com/ansible/ansible) playbook.

## Example playbook

Example use of a role, that will install the latest version of [DDEV](https://ddev.readthedocs.io/en/stable).

```yml
- hosts: all
  roles:
    - role: krudi.ddev
      ddev:
        install: true
```

## Issue

Have you found a bug in this project or have a suggestion for a new feature? Create a new ticket for the bug or feature, which can be found on the [GitHub](https://github.com/krudi/ansible-role-ddev/issues) page.
