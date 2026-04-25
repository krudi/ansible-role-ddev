# Ansible Role — DDEV

Ansible role that installs DDEV and its Docker dependency on target hosts.

@AGENTS.md

## For Claude Code

### Rules loaded automatically

| Rule file | Applied to |
|-----------|---|
| `.ai/rules/ansible.md` | `**/*.yml`, `**/*.yaml` |

### Constraints

- Commits use conventional commits format (see global `AGENTS.md`)
- Role installs DDEV **and** Docker as a dependency — check `defaults/main.yml` for version variables
- Tasks run as a privileged user — ensure privilege escalation is handled via `become`
- Test with `molecule test` before merging changes that affect idempotency
