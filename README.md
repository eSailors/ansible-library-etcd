ansible-library-etcd
------------------

# Description
Ansible library to manage Etcd keys.

# Requirements
[python-etcd] is required to be installed.

# Usage
Ensure a key is present
```
- name: Ensure Etcd key
  etcd_key:
    name: myKey
    value: myValue
    ttl: 10
    state: present
    etcd_host: etcd.example.com
    etcd_port: 4001
```
Ensure a key is absent
```
- name: Ensure Etcd key
  etcd_key:
    name: myKey
    state: absent
    etcd_host: etcd.example.com
    etcd_port: 4001
```

# Author information
[Thomas Krahn]

[python-etcd]: https://github.com/jplana/python-etcd
[Thomas Krahn]: mailto:ntbc@gmx.net
