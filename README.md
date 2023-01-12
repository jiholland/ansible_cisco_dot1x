🔐 csico\_dot1x
===============

Configure 802.1X.

Requirements
------------

💿 [Cisco IOS Collection](https://galaxy.ansible.com/cisco/ios)

Role Variables
--------------

- radius\_server\_group
- radius\_server\_key
- radius\_server\_primary\_name
- radius\_server\_primary\_ip
- radius\_server\_secondary\_name
- radius\_server\_secondary\_ip
- interface\_authentication\_order
- interface\_authentication\_priority
- interface\_authentication\_multi\_auth
- device\_sensors

Dependencies
------------

None.

Example Playbook
----------------

    ---
    - name: Configure 802.1X.
      hosts: "{{ target }}"
      gather_facts: true

      roles:
        - role: cisco_dot1x
          tags: dot1x

License
-------

BSD

Author Information
------------------

Jørn Ivar Holland
