# ansible-role-ddev

A role for [Ansible](https://github.com/ansible/ansible), that installs [DDEV](https://ddev.readthedocs.io/en/stable) for launching local PHP development environments.

## Requirements

This role does not need any additional required packages

## Dependencies

- The only dependencies needed for this role is [ansible-role-docker](https://github.com/geerlingguy/ansible-role-docker) from [geerlingguy](https://github.com/geerlingguy), which is built into this role

## Quick start

1. First clone this repository and add into your project directory
2. Include the role in your [Ansible](https://github.com/ansible/ansible) playbook

## Example playbook

Example use of a role, that will install the latest version of [DDEV](https://ddev.readthedocs.io/en/stable)

```yml
- hosts: all
  roles:
    - role: krudi.ddev
```

## Linting commands for [yamllint](https://yamllint.readthedocs.io/en/stable/quickstart.html)

If you have [yamllint](https://yamllint.readthedocs.io/en/stable/quickstart.html) installed on your machine then here are some useful commands for linting .yml files

- `yamllint .` - to lint all YAML files in a whole directory
- `yamllint -c ./.yamllint .` - to lint all YAML files in a whole directory with specifed configuration

## Issue

Have you found a bug in this project or have a suggestion for a new feature? Create a new ticket for the bug or feature, which can be found on the [GitHub](https://github.com/krudi/ansible-role-ddev/issues) page
