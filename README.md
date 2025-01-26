# Ansible Role: Neovim

[![CI](https://github.com/pluggero/ansible-role-neovim/actions/workflows/ci.yml/badge.svg)](https://github.com/pluggero/ansible-role-neovim/actions/workflows/ci.yml) [![Ansible Galaxy downloads](https://img.shields.io/ansible/role/d/pluggero/neovim?label=Galaxy%20downloads&logo=ansible&color=%23096598)](https://galaxy.ansible.com/ui/standalone/roles/pluggero/neovim)

An Ansible Role that installs a basic configuration of Neovim.

## Requirements

Requires an installation of lazygit; Recommended role: `pluggero.lazygit`.
Requires an installation of netcoredbg.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - pluggero.neovim
```

## License

MIT / BSD

## Author Information

This role was created in 2025 by Robin Plugge.
