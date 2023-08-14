Role Name
=========

Whitelisting

Requirements
------------

Python, Ansible 7.0.0

Role Variables
--------------

Role for parse Jira for whitelisting tasks and do whitelisting in Fortigate

Dependencies
------------

ansible.posix, community.general, fortinet.fortios:2.2.0

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: Parse Jira and Do Whitelist tasks
      hosts: fortigates
      gather_facts: no
      connection: httpapi
      roles:
        - whitelisting

License
-------

MIT

Author Information
------------------

Danila Eliseev
SB2 Team DevOps Engineer