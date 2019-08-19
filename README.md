# Ansible Role: Nexus

## Summary

  This role installs Nexus Repository Manager and required packages.

## Role tasks

  - Create user/group for Nexus service to run as
  - Create directories for Nexus
  - Download and verify tar file
  - Render config files from templates
  - Create Nexus SystemD service
  - Add FirewallD service for Nexus

## Requirements

  Host should be previously bootstrapped preferable with ansible-role-bootstrap

## Role Variables

  All variables are listed in defaults/main.yml along with their default values

## Dependencies

  None.

## Example Playbook

```yaml
  ---

  - name: Apply role ansible-role-nexus to every host in group 'all'
    hosts: all
    roles:
      - role: ansible-role-nexus

```

## License

MIT

## Author Information

Author:
  - Max Khmelevsky <max.khmelevsky@yandex.ru>
