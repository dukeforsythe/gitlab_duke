ansible-role-dns
================

Ansible role for configure DNS

# Examples :
```
- hosts: dev
  roles: 
  - role: ansible-role-dns
    dns_domain: dev.nonprod
    dns_nameservers: ['10.130.10.64']
    dns_searchs: "qa.nonprod dev.nonprod"

- hosts: qa
  roles:
  - role: ansible-role-dns
    dns_domain: qa.nonprod
    dns_nameservers: ['10.130.10.64']  
    dns_searchs: "qa.nonprod dev.nonprod"

```
