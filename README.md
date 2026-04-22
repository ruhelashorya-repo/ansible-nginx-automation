# Ansible Nginx Automation Lab

This project automates the configuration of an Azure-hosted Ubuntu Linux VM using Ansible.

## What this playbook does

- Connects to a remote Azure Linux VM over SSH
- Updates the apt package cache
- Installs Nginx
- Starts and enables the Nginx service
- Deploys a custom HTML landing page
- Restarts Nginx to apply changes

## Tools used

- Ansible
- Azure Virtual Machine
- Ubuntu Linux
- Nginx
- WSL (Ubuntu on Windows)

## Files

- `hosts` — inventory file with target VM details
- `install_nginx.yml` — Ansible playbook
- `README.md` — project documentation

## How to run

```bash
ansible-playbook -i hosts install_nginx.yml --ask-become-pass