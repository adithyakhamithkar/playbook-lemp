# Deploy the LEMP Stack on Ubuntu 14.04 using Ansible playbook
## Setting up an Ansible workstation on Ubuntu 14.04
These are the instructions for Ubuntu 14.04
```sh
apt-get update
apt-get install python-pip python-dev git -y
pip install PyYAML jinja2 paramiko
git clone https://github.com/ansible/ansible.git
cd ansible
make install
mkdir /etc/ansible
cp ~/ansible/examples/hosts /etc/ansible/
```
## Clone the Repo and edit make a copy of the hosts_template file as hosts and run
```sh
ansible-playbook -i hosts main.yml
```
