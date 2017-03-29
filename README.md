# Disable transparent huge pages

For use on linux, on sb servers (redis, cassandra, mongodb, etc)

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