k8s-registry-credentials
=========

Role for ansible. Create kubernetes secret for pull image from docker registry

Role Variables
--------------

* namespace - Namespace for creation secret
* secret_name - Name of secret entity (Default: registry-credentials)
* registry_name - Registry hostname (Example: registry.gitlab.com)
* username - Registry auth username 
* password - Registry auth password
* email - Email for registry

Example Playbook
----------------

    - hosts: deploy
      roles:
         - { role: amaxlab.k8s-registry-credentials, namespace: default, username: test, password: test, registry_name: registry.gitlab.com, email: test@test.ru}

License
-------

MIT
