# Ansible Role: Neovim

[![CI](https://github.com/pluggero/ansible-role-neovim/actions/workflows/ci.yml/badge.svg)](https://github.com/pluggero/ansible-role-neovim/actions/workflows/ci.yml) [![Ansible Galaxy downloads](https://img.shields.io/ansible/role/d/pluggero/neovim?label=Galaxy%20downloads&logo=ansible&color=%23096598)](https://galaxy.ansible.com/ui/standalone/roles/pluggero/neovim)

An Ansible Role that installs a basic configuration of Neovim.

## Requirements

Requires an installation of lazygit; Recommended role: `pluggero.lazygit`.
Requires an installation of netcoredbg.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
neovim_version: "x.x"
```

The version of neovim to install can be defined in the variable `neovim_version`.

```yaml
neovim_install_method: "dynamic"
```

The method used to install neovim can be defined in the variable `neovim_install_method`.
The following methods are available:

- `source`: Installs neovim from source
- `package`: Installs neovim from the package manager of the distribution
  - **NOTE**: This method installs the latest version available in the package manager and not the version defined in `neovim_version`.
- `dynamic`: Installs neovim from package manager if available in the correct version, otherwise installs from source

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
