Role Name
=========

This is a app-tier role for tomcat.

Requirements
------------

1) git repository: https://github.com/bsk1072/ansible_advance_homework.git
2) Playbooks to deploy internal 3-tier app
3) Install HA Ansible Tower

Role Variables
--------------

the variables are usually inside the vars/main.yml
example: 
    payload:          tomcat
    tomcat_web_root:  /usr/share/tomcat/webapps/ROOT

Dependencies
------------

Should be linux, Python should be installed as same version to Ansible server to avoid the modules compactibility issues
Ansible control should be able to communicate with the host.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

        - name: create tomcat default web directory
          file:
            path: "{{ tomcat_web_root }}"
            state: directory

License
-------

Opensource

Author Information
------------------

bsk1072 | studydevops.blogspot.com
