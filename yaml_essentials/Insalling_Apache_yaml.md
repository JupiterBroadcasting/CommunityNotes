# Installing Apache On Ubuntu 18.04

## Ansible:
```
--- # This is a YAML structure example
- hosts: localhost
  remote_user: ansible
  become: yes
  become_method: sudo
  connection: ssh
  gather_facts: yes
  tasks:
    - name: Install Apache
      apt:
        name: apache2
        state: latest
      notify:
        - startservice
  handlers:
    - name: startservice
      service:
        name: apache2
        state: restarted
```

## Salt 

```
install_apache:
  pkg.installed:
    - name: apache2
  service.running:
    - name: apache2
```