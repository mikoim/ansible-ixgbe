ansible-ixgbe
=========

[![Build Status](https://travis-ci.org/mikoim/ansible-ixgbe.svg?branch=master)](https://travis-ci.org/mikoim/ansible-ixgbe)


Install ixgbe driver for Intel 10 Gigabit Ethernet Network Connections.

Requirements
------------

On general Linux environments, requires kernel headers and build tools.

Role Variables
--------------

```yaml
# Installation options.
ixgbe_version: 4.4.6
ixgbe_download_url: "https://downloadmirror.intel.com/14687/eng/ixgbe-{{ ixgbe_version }}.tar.gz"
ixgbe_checksum: md5:e11e83c96afe846b5ee72c309a58e11f

# If set true, reload ixgbe module after installing.
ixgbe_reload_module: false
```

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: mikoim.ixgbe }
```

License
-------

GPLv2
