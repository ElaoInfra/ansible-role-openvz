<img src="http://www.elao.com/images/corpo/logo_red_small.png"/>

# Ansible Role: OpenVZ

This role will assume the setup of OpenVZ

It's part of the ELAO [Ansible stack](http://ansible.elao.com) but can be used as a stand alone component.

## Requirements

- Ansible 1.7.2+

## Dependencies

None.

## Installation

Using ansible galaxy:

```bash
ansible-galaxy install elao.openvz
```
You can add this role as a dependency for other roles by adding the role to the meta/main.yml file of your own role:

```yaml
dependencies:
  - { role: elao.openvz }
```

## Role Variables

|Name|Default|Type|Description|
|----|-------|----|-----------|

### Configuration example

```yaml

elao_openvz_templates_exclusive: true
elao_openvz_templates:
  - http://download.proxmox.com/appliances/system/debian-7.0-standard_7.0-2_amd64.tar.gz

```

## Example playbook

    - hosts: servers
      roles:
         - { role: elao.openvz }

# Licence

MIT

# Author information

ELAO [**(http://www.elao.com/)**](http://www.elao.com)
