# Ansible Role : Transparent Huge Pages

An Ansible Role to set the transparent huge pages mode.

## Role Variables:

Available variables are listed below, along with the default values (see `defaults/main.yml`):

    mode: never

    values:
      never
      always
      madvise

## Dependencies

None.

## Example Playbook

    - hosts: kubernetes-nodes
      var_files:
      - vars/main.yaml
      roles:
      - 'transparent-hugepages'
