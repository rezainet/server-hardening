# server-hardening

Ansible roles that bring a fresh Ubuntu 22.04/24.04 server close to the CIS Benchmark, plus an audit script that scores the machine before and after.

## What it does

- SSH, PAM and sudo policy
- Filesystem mount options and permissions
- Kernel and network sysctl, host firewall
- auditd and logging
- Removal of unused services and packages

## Results (clean Ubuntu 24.04 VM)

| | Score |
|---|---|
| Before | to be filled from a clean VM |
| After | to be filled from a clean VM |

Full audit output will be in docs/before-after.md.

## Usage

```bash
ansible-playbook -i inventory/lab.yml playbooks/harden.yml
./scripts/cis_audit.sh
```

## Notes

Built from work hardening a production server to 99.56% CIS compliance. This repository contains only generic, lab-tested roles. No customer or company data.

## Status

Roles are being published one at a time from September 2026.
