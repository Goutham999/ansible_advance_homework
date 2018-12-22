Role Name
=========

This is a base-config role does the below,

        1) enable sudo without tty for some ansible commands
        2) enable repos
        3) install base tools and packages

Requirements
------------
  1) Ansible Tower Homework Lab
  2) OpenStack for Ansible
  3) Ansible Advanced
  4) https://github.com/bsk1072/ansible_advance_homework.git

Role Variables
--------------

    1) export TOWER_GUID=ccd4
    2) export MYKEY=~/.ssh/mykey.pem
    3) export MYUSER=bhandari-santhosh.kumar-atos.net

Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

        - name: enable repos
          template:
            src: repos_template.j2
            dest: /etc/yum.repos.d/open_three-tier-app.repo
            mode: 0644

License
-------

BSD

Author Information
------------------

bsk1072 | [studydevops.blogspot.com](http://studydevops.blogspot.com/)
