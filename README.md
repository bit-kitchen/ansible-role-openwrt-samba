ansible-role-openwrt-samba
==========================

Configure OpenWrt for samba server.

Requirements
------------

None.

Role Variables
--------------

Variable   | Default | Comment
---------- | ------- | -------
samba_luci | yes     | Install samba luci app
samba_wsd  | yes     | Install wsdd2 for [WSD](https://en.wikipedia.org/wiki/Web_Services_for_Devices) support which enables file share discovery on Windows

Dependencies
------------

* `gekmihesg.openwrt`
* `bit_kitchen.openwrt_storage`

Example Playbook
----------------

```yml
- hosts: openwrt
  remote_user: root
  gather_facts: no
  roles:
  - bit_kitchen.openwrt_samba
```

License
-------

[MIT](LICENSE)

Author Information
------------------

[bit.kitchen](https://github.com/bit-kitchen)
