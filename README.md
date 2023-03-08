# ansible-role-patch_linux

Ansible role for patching linux servers. Will check for kernel and package updates, will only reboot if kernel updates were applied.


## Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

This should contain the exact same content that is in the `requirements.txt` file.

```
hvac
```

## Role Variables

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

> NOTE: It is important to have unique variables in all of your roles -- or you run the risk of having duplicate variables. You should prefix the role name to any variable you define. E.g. `example_role_name_my_variable`

```yml
---
example_role_name_my_variable: myValue
```

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

This should contain the exact same content that is in the `requirements.yml` file.

```yml
---
collections:
  - name: community.windows
roles:
  - name: ansible-role-windows_update
    src: https://github.com/jeffbildz/ansible-role-windows_update.git
    scm: git
    version: devel
```

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
---
- hosts: servers
  roles:
    - ansible-role-patch_linux
```

## License

BSD

## Author Information

Contributors:

- Mike Fann (mfann@jeffbildz.com)

Please consider contributing back to this project. https://github.com/jeffbildz/ansible-role-template
