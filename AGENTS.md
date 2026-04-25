# Ansible Role — DDEV

Ansible role that installs DDEV (Docker-based PHP development environment) and its Docker dependency.

## Stack

- Ansible / YAML

## Commands

```bash
ansible-lint       # lint the role
molecule test      # full test (if molecule configured)
```

## Onboarding

**Prerequisites:** Ansible, Python, molecule (for testing).

1. `ansible-lint` — verify the role passes linting
2. `molecule converge` — apply the role to a test instance
3. `molecule test` — full test including idempotency check

---

## Testing

- Run before every PR: `ansible-lint && molecule test`
- Idempotency is required: running the role twice must produce no changes
- Test on both Debian/Ubuntu and RHEL if changes affect platform-specific tasks

---

## Notes

- Depends on a Docker role — ensure Docker is installed before this role runs
- DDEV version is controlled by a role variable (see `defaults/main.yml`)

---

## Rules

@.ai/rules/ansible.md
