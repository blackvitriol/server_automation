# server_automation
Using Ansible to perform system update, install latest ngnix and latest nodejs.

## how to use 
### (pre-requisities)
This is intended to be used on a Ubuntu 18.04 system.
On the master computer, open a terminal and add:
> sudo apt-add-repository ppa:ansible/ansible &&
> sudo apt update &&
> sudo apt install ansible

Edit the configurations to add remote computers:
> sudo nano /etc/ansible/hosts

Test your connections to remote computers:
> ansible all -m ping -u remote_user
> ansible all -a "df -h" -u root 

### load this project
On the master computer, open a terminal and run:
> git clone <this repos address>
  
