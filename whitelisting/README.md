Role Name
=========

Whitelisting

Requirements
------------

Python, Ansible

Role Variables
--------------

*jira_server* - url of your company Jira server
*jira_user/token* - creds for using Jira via API


*target_label* - label in Jira for found tasks to do
*target_status* - status in Jira for sort done and to do tasks
*target_project* - project in Jira where we will create tasks for whitelisting

*vdom* - Fortigate VDOM where we do routing and whitelisting
*fortigate_token* - Fortigate API Access Token for manage rules

Role for parse Jira for whitelisting tasks and do whitelisting in Fortigate

Dependencies
------------

ansible.posix, community.general, fortinet.fortios:2.2.0

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: Parse Jira and Do Whitelist tasks
      hosts: fortigate
      gather_facts: no
      connection: httpapi
      roles:
        - { role: ../whitelisting }

License
-------

MIT

Author Information
------------------

Danila Eliseev
DevOps Engineer