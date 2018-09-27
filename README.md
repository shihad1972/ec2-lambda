ec2-lambda
=========

Create a lambda function within the AWS cloud

Requirements
------------

Boto will be required for this role

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

 This has a dependency on the ec2-iam role. This is required, so the lambda function can access AWS resources. You will be required to pass in 2 policy documents, JSON formatted, 1 to describe the trust relationship and 1 that contains the IAM policy.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GPL

Author Information
------------------

Iain M. Conochie <iain@thargoid.co.uk>
