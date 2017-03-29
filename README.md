# Disable transparent huge pages

For use on linux, on db servers (redis, cassandra, mongodb, etc)

See https://docs.mongodb.com/v3.2/tutorial/transparent-huge-pages/ for details.

## Requirements

Ansible 2+

## Dependencies

None

## Examples

```YAML
- hosts: all
  roles:
    - role: ansible-transparent-huge-pages
```

```YAML
- hosts: all
  roles:
    - role: ansible-transparent-huge-pages
      start_before: 
        - redis
        - sentinel
```
