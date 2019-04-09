Ansible Role: tamay.docker-ce
=========

This role installs the docker community edition.

Requirements
------------

None.

Role Variables
--------------

List of all variables, including default values.

    docker_users: []

List of users that will be added to the unix group ```docker```. The user will be created if it does not exist.
    


Dependencies
------------

None.

Example Playbook
----------------

    ---
    
    - hosts: all
      remote_user: vagrant
      become: yes
    
      vars:
        docker_users:
          - user1
          - user2
    
      roles:
      - ../../tamay.docker-ce

License
-------

MIT

Author Information
------------------

tamay.mueller@gmail.com