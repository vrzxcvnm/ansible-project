# ansible-project

Ansible-based automation project for the practical exam.

## What it does
- Installs Docker Engine and Docker Compose plugin on Ubuntu
- Enables and starts the Docker service
- Deploys an Nginx container via docker compose that serves index.html on port 80

## Project structure
- roles/install_docker
- roles/run_nginx_website
- playbook.yaml
- .github/workflows/ansible-validate.yml

## How to run locally

```bash
sudo apt update
sudo apt install -y ansible
sudo ansible-playbook -i inventory.ini playbook.yaml
```
## Verify

```bash
curl http://localhost
sudo docker ps
```
