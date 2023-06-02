# swarm-setup-ansible
Ansible Playbook to install and configure Docker Swarm

Changes with each Deployment:

- network interface in /roles/swarm/tasks/main.yml
- roles/docker/main.yml "Add user to docker group"
- 
To run playbook
```
ansible-playbook -i inventory/hosts.yml -u user -K install-swarm.yml
```
Inspiration from:
https://gitlab.com/xavki/devopsland/-/tree/master/ansible/vagrant
https://xavier-pestel.medium.com/an-easy-way-to-install-a-docker-swarm-cluster-with-ansible-ebebada3c116
