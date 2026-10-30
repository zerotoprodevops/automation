# Ansible Server Baseline & Configuration

This repository contains the Ansible automation used to provision and configure RHEL 10 servers for AcmeCorp.

## Project Structure
- `site.yaml`: The main entry point playbook.
- `roles/common`: Baseline packages for all servers.
- `roles/firewall`: Standardized Firewalld configuration.
- `roles/webserver`: Apache (httpd) configuration for Web nodes.
- `roles/database`: MariaDB configuration for DB nodes.
- `group_vars/`: Environment and group-specific variables.

## Usage
To run the playbook:
```bash
ansible-navigator run site.yaml -m stdout