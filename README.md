# Arch Linux Core Pacman Packages Task Module

This Ansible task module handles the installation and management of core pacman
packages for Arch Linux systems.

## Overview

This module:

- Installs a configurable set of essential Arch Linux packages

## Requirements

- Ansible 2.9+
- Target system running Arch Linux or an Arch-based distribution
- Root/sudo privileges on the target system
- Internet connectivity for package downloads

## Usage

Example inclusion in a playbook:

```yaml
- name: Install Arch Linux core packages
  include_tasks: tasks/task-pacman-core.yml
```

## Dependencies

This module has no external dependencies beyond the core Ansible requirements.

## Notes

- This module is idempotent and will only install packages that aren't already present
- Package lists can be extended or overridden with your own custom lists
