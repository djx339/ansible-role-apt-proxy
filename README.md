Ansible Role: APT Proxy
=========

Set http/https/no proxy for apt.

Requirements
------------

None.

Role Variables
--------------

```yaml
proxy_env:
  http_proxy: http://proxy.example.com:8080
  https_proxy: http://proxy.example.com:8081
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: all
  become: yes
  vars:
    proxy_env:
      http_proxy: http://proxy.example.com:8080
      https_proxy: http://proxy.example.com:8081
  roles:
    - { djx339.apt-proxy }
```

License
-------

BSD

Author Information
------------------

This role was created by [Daniel D](https://github.com/djx339).
