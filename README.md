# AWS RHEL 9 Infrastructure Automation with Ansible

## Architecture
Internet → AWS Application Load Balancer → 2x RHEL 9 EC2 (Nginx)
Configuration fully automated via Ansible from a dedicated control node.

## What This Demonstrates
- AWS EC2 provisioning and networking (Security Groups, ALB, Target Groups)
- Ansible playbook design (idempotent, using proper ansible.cfg)
- RHEL 9 service management (Nginx, firewalld)
- Real-world troubleshooting: collection path issues, missing 
  firewalld config on minimal cloud images, Git/GitHub auth setup

## Files
- `nginx_setup.yml` — Main Ansible playbook
- `ansible.cfg` — Ansible configuration (inventory, collections, roles paths)
- `inventory.ini` — Host inventory (not committed, contains real IPs)

## Skills Used
AWS EC2, AWS ALB, AWS Target Groups, Security Groups, RHEL 9, 
Ansible, Ansible Collections (ansible.posix), Nginx, firewalld, Git/GitHub

## Author
Parth Mistri | Senior Linux System Administrator | RHCE & RHCSA Certified
