Role Name
=========

An example ansible roles for create instance on GCP.

Requirements
------------

- python >= 2.6
- apache-libcloud >= 0.13.3, >= 0.17.0 if using JSON credentials, >= 0.20.0 if using preemptible option

Role Variables
--------------

server_name = for instance name
service_account = your service account
credentials_file = file path to json file for auth
project_id = project id

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      vars:
        server_name: server-1
        service_account: xxxxxxx-compute@developer.xxxxxxxx
        json_file: ../templates/auth.json
        project_name: tensile-XXXXX-XXXXX
      roles:
         - { role: gcp }

License
-------

GPLv3

Author Information
------------------

elasyaf @ 2018
