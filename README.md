# pg_repo

Sets up upstream PostgreSQL repositories on RHEL/Fedora.

## Role Variables

- `postgresql_version` major PG version, defaults to 14.

## Example dependency

```yml
dependencies:
  - name: cosandr.pg_repo
    src: https://github.com/cosandr/ansible-role-pg_repo.git
    scm: git
    version: v1.0.0
```

## Example Playbook

```yml
    - hosts: servers
      roles:
         - { role: cosandr.pg_repo, postgresql_version: 13 }
```

## License

MIT

## Author Information

Andrei Costescu

## Credits

[Jeff Geerling](https://github.com/geerlingguy/ansible-role-postgresql)
