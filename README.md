bamboo
======

Installs Bamboo

Requirements
------------

This role requires Ansible 1.6 or higher.

Role Variables
--------------

| Name                     | Default                                                          | Description                  |
|--------------------------|------------------------------------------------------------------|------------------------------|
| bamboo_version           | 5.8.1                                                            | Version of Bamboo to install |
| bamboo_archive_sha256sum | bb691d22273ceaa999eb435dfb4e8d697c3c803505218845bf5785ec2785cbd8 | SHA 256 checksum of archive  |

Dependencies
------------

- kbrebanov.java (Java 8)

Example Playbook
----------------

Install Bamboo
```
- hosts: all
  roles:
    - { role: kbrebanov.bamboo }
```

Install Bamboo specifying version
```
- hosts: all
  roles:
    - { role: kbrebanov.bamboo, bamboo_version: 5.8.0 bamboo_archive_sha256sum: 88e2463a775fe6078c6ccf5142117384beb0be4d73815ce2146e0f05cde771f5 }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov