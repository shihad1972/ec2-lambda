ec2-lambda
=========

Create a lambda function within the AWS cloud

Requirements
------------

Boto will be required for this role

Role Variables
--------------

See the example playbook below for the variables to pass into this role

Dependencies
------------

 This has a dependency on the ec2-iam role. This is required, so the lambda function can access AWS resources. You will be required to pass in 2 policy documents, JSON formatted, 1 to describe the trust relationship and 1 that contains the IAM policy.

Example Playbook
----------------

    - hosts: localhost
      vars:
        template_dir: some/path/to/your/templates
        iam_templates:
          - role: iam_role_document.json
            policy: iam_policy_document.json
            name: name_of_iam_role
            managed: []
            type: role
      roles:
        - ec2-lambda

License
-------

GPL

Author Information
------------------

Iain M. Conochie <iain@thargoid.co.uk>
