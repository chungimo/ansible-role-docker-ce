Ansible Role for Docker-CE
=========

Ansible role to install Docker CE and Docker Compose.

* Working on Redhat-family and Ubuntu distributions.
* Define {{ docker_bip_ip }} in defaults/main.yml if you set docker_override_ip to true from the playbook.

Example Playbook
----------------
```yaml
    - hosts: servers
      gather_facts: true
      vars:
        docker_override_ip: True
      roles:
        - role: docker-ce
```
