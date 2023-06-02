# swarm-setup-ansible
Ansible Playbook to install and configure Docker Swarm

make sure to change network interface to proper one on /roles/swarm/tasks/main.yml

To run playbook
```
ansible-playbook -i inventory/hosts.yml -u user -K install-swarm.yml
```
Inspiration from:
https://gitlab.com/xavki/devopsland/-/tree/master/ansible/vagrant
https://xavier-pestel.medium.com/an-easy-way-to-install-a-docker-swarm-cluster-with-ansible-ebebada3c116
