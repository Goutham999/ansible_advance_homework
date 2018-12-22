Role Name
=========

This role does the follow below,
    1) Create new server instances and attaches them a network and passes metadata to the instance.
    2) Add floating IP to Servers
    3) OpenStack servers
    4) Wait for server to be available
    5) 

Requirements
------------

  1) Ansible Tower Homework Lab
  2) OpenStack for Ansible
  3) Ansible Advanced
  4) https://github.com/bsk1072/ansible_advance_homework.git

Role Variables
--------------

export TOWER_GUID=ccd4
export MYKEY=~/.ssh/mykey.pem
export MYUSER=bhandari-santhosh.kumar-atos.net

Dependencies
------------

  1) {{tower_guid}} is the GUID (unique identifier) i.e ccd4
  2) {{osp_guid}} is the GUID for workstation machine i.e 7e66

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

        - name: OpenStack servers
          os_server_facts:
            cloud: ospcloud
          register: result
          tags:
            - test.servers

License
-------

Opensource

Author Information
------------------

bsk1072 | [studydevops.blogspot.com](http://studydevops.blogspot.com/)
