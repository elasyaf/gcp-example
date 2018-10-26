Role Name
=========

An example ansible roles for create instance on GCP.

Requirements
------------

- python >= 2.6
- apache-libcloud >= 0.13.3, >= 0.17.0 if using JSON credentials, >= 0.20.0 if using preemptible option

Role Variables
--------------

- server_name = for instance name
- service_account = your service account
- json_file = file path to json file for auth
- project_name = project id

Dependencies
------------

None

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
