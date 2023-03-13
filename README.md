🔐 cisco\_dot1x
===============

Configure 802.1X.

Requirements
------------

💿 [Cisco IOS Collection](https://galaxy.ansible.com/cisco/ios)

Role Variables
--------------

- dot1x\_radius\_server\_group
- dot1x\_radius\_server\_key
- dot1x\_radius\_server\_primary\_name
- dot1x\_radius\_server\_primary\_ip
- dot1x\_radius\_server\_secondary\_name
- dot1x\_radius\_server\_secondary\_ip
- dot1x\_interface\_authentication\_order
- dot1x\_interface\_authentication\_priority
- dot1x\_interface\_authentication\_multi\_auth
- dot1x\_radius\_server\_attributes
- dot1x\_device\_sensors

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
        - role: dot1x
          tags: dot1x

License
-------

BSD

Author Information
------------------

Jørn Ivar Holland
