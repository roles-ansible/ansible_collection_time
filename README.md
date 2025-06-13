[![collection l3d.time](https://ansible.l3d.space/svg/l3d.time_ansible-collection_collection.svg)](https://galaxy.ansible.com/ui/repo/published/l3d.time/)
[![Maintainance](https://ansible.l3d.space/svg/l3d.time_maintainance_collection.svg)](https://ansible.l3d.space/#l3d.time)
[![License](https://ansible.l3d.space/svg/l3d.time_license_collection.svg)](LICENSE)

 Ansible Collection - l3d.time
============================

This is the Ansible Collection ``l3d.time``. A collection for our time manupulating ansible roles.
Here are all our ansible roles for installing git server.

## Ansible Roles in l3d.time
- [![l3d.time.ntp](https://ansible.l3d.space/svg/l3d.time.ntp_ansible-role.svg)](https://github.com/roles-ansible/ansible_role_ntp.git) - Ansible role to install and configure the Network Time Protocol (NTP) Daemon.

## Using this Collection
You can install the collection using ansible-galaxy by running:
```bash
ansible-galaxy collection install l3d.time:1.0.4
```

Remember you can to Upgrade to the latest version of the l3d.time collection using the ``--upgrade`` parameter:
```bash
ansible-galaxy collection install l3d.time --upgrade
```


Or you could clone this collection in your local ansible project for example to ``collections/ansible_collections/l3d.time/``. Make sure you checkout [git submodules](https://git-scm.com/docs/git-submodule) too. Example:
```
# Clone git Repo with submodules to specified path
git clone --recursive https://github.com/roles-ansible/ansible_collection_time.git collections/ansible_collections/l3d/time/

# change directory
cd collections/ansible_collections/l3d.time/

# optionally init git submodules
git submodule update --init --recursive

# optionally install all requirements
ansible-galaxy collection install -r requirements.yml --upgrade
```

You can also list a collection in ``requirements.yml``:
```yaml
---
collections:
  - name: l3d.time
    version: ">=1.0.4"
```

## Include roles in your playbook
Example Playbook using the l3d.time.ntp role:
```yaml
---
- name: "Install NTP Server from collection l3d.time"
  hosts: ntp.example.com
  roles:
    - {role: l3d.time.ntp, tags: ntp}
  vars:
    ntp_set_time_zone: true
    ntp_timezone: Zulu
```

## Requirements
The roles in this collection using the ``community.general`` ansible Collections.

### Example Requirements Installation:
```bash
# galaxy requirements
ansible-galaxy install -r requirements.yml --upgrade
```
