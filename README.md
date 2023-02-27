buat file host dengan nama inventory

cek akses > ansible host -i inventory -m ping

ansible [host] -m ping >> /etc/ansible/host
masukan cred [host:vars]

[host:vars]
ansible_connection=ssh
ansible_user=oce
#ansible_password=123123
#ansible_ssh_private_key_file=~/.ssh/ansible

###how to play with sudo access
ansible-playbook -i inventory playbook-user.yml -kK