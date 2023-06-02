# swarm-setup-ansible
Ansible Playbook to install and configure Docker Swarm 
*tested on Ubuntu 22.04


Requirements:
- Ansible installed on local machine or Control Node
- SSH enabled on each server
- Fingerprint from from each server (i.e. login to each with ssh or ssh-copy-id user@ipaddress)


Changes with each Deployment:

- network interface in /roles/swarm/tasks/main.yml
- roles/docker/main.yml "Add user to docker group"
- inventory/hosts.yml to specified IP Addresses


To run playbook
```
ansible-playbook -i inventory/hosts.yml -u user -K install-swarm.yml
```
Inspiration from:
https://gitlab.com/xavki/devopsland/-/tree/master/ansible/vagrant
https://xavier-pestel.medium.com/an-easy-way-to-install-a-docker-swarm-cluster-with-ansible-ebebada3c116
