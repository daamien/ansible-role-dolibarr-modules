Role Name
=========

![Ansible Lint](https://github.com/daamien/ansible-role-dolibarr-modules/workflows/Ansible%20Lint/badge.svg)
![YAML Lint](https://github.com/daamien/ansible-role-dolibarr-modules/workflows/Yaml%20Lint/badge.svg)

Manage Dolibarr modules

Role Variables
--------------

* dolibarr_module (see default/main.yml)
* dolibarr_module_path: local path to your version of the module
* dolibarr_env:  i the FQDN of your dolibarr environment


Example Playbook
----------------

```yaml
  vars:
    dolibarr_module: my-module
    dolibarr_module_path: ~/dev/dolibarr/my-module
    dolibarr_env: my.dolibarr-server.com

  tasks:
    - name: Deploy
      import_role:
        name: dolibarr_modules
        tasks_from: deploy
```

License
-------

BSD

