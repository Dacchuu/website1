# Ansible Configuration Management

This project uses Ansible to automate infrastructure setup.

## Roles

### Jenkins Server
- Java installation
- Jenkins installation
- Jenkins service setup

### Kubernetes Nodes
- Docker installation
- Kubernetes tools installation (kubectl)

## Execution

Run playbook:

```bash
ansible-playbook -i inventory.ini site.yml
