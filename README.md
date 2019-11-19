# Ansible Role: Users

[![Gitlab pipeline status (self-hosted)](https://git.dubzland.net/dubzland/ansible-role-users/badges/master/pipeline.svg)](https://git.dubzland.net/dubzland/ansible-role-users/pipelines)

Configures users and groups on linux based systems.

## Requirements

Ansible version 2.0 or higher

## Role Variables

Available variables are listed below, along with their default values (see `defaults/main.yml` for more info):

### dubzland_users_admin_group

```yaml
dubzland_users_admin_group: admin
```

Group allowed to execute sudo without a password.

### dubzland_users_admin_default_password

```yaml
dubzland_users_admin_default_password: notsekret
```

Password to assign to newly created admin users.

### dubzland_users_admins

```yaml
dubzland_users_admins: {}
```

List of admin users to add to the system.

### dubzland_users

```yaml
dubzland_users: {}
```

List of normal users to add.

## Dependencies

None

## Example Playbook

```yaml
- hosts: all
  roles:
    - role: dubzland.users
```

## License

MIT

## Author

* [Josh Williams](https://codingprime.com)
