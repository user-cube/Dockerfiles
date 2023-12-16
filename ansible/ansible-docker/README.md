# Ansible Docker
This docker image allows you to run ansible playbooks on your local docker machine.

## Build

```bash
docker build -t ruicoelho43/ansible:latest .
```

## Execute

To execute the ansible playbook run the following command:

```bash
docker run  -v "${PWD}":/work:ro --rm ansible ansible-playbook my-playbook.yaml
```
