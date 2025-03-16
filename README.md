# LearnAnsible
This is for learning basics ansible

#Run manually

ansible -i inv all -e  ansible_user=ec2-user -e  ansible_password=DevOps321 -m ansible.builtin.shell -a  "df -h"
ansible -i inv all -e  ansible_user=ec2-user -e  ansible_password=DevOps321 -m ansible.builtin.shell -a  free
ansible -i inv all -e  ansible_user=ec2-user -e  ansible_password=DevOps321 -m ansible.builtin.shell  -a top

ansible -i inv dev -e  ansible_user=ec2-user -e  ansible_password=DevOps321 -m ansible.builtin.shell  -a "mkdir dev-inventory"
ansible -i inv prod -e  ansible_user=ec2-user -e  ansible_password=DevOps321 -m ansible.builtin.shell  -a "mkdir prod-inventory"

YAML BASICS

- name: AnsiblePlaybook
  hosts: dev
  tasks"
  - name: playbook1 and task1
    ansible.builtin.ping
     msg: "Hello world"


From Machine

ansible-playbook -i inv -e ansible_username=ec2-user   -e ansible_password=DevOps321 01-playbook.yml
  
    