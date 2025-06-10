# Ansible Playbooks

This repository contains Ansible playbooks and related files. The `playbooks/ap_trunk_config.yml` playbook automatically configures switch ports connected to Cisco access points based on CDP discovery data. The playbook uses the `cisco.ios` collection and is compatible with AWX or Ansible Tower.

## Usage

Run the playbook against your switch inventory:

```bash
ansible-playbook -i inventory playbooks/ap_trunk_config.yml
```

The inventory should define the target switches using the `network_cli` connection.


