**#sshkey for host** 

generate sshkey, kemudian lakukan ssh-copy-id ke host tujuan > agar ansible dapat tersambung ke host

**#host file**

create file host dengan nama inventory

**#connection check**

cek akses > ansible host -i inventory -m ping

**#how to play with sudo access**

ansible-playbook -i inventory playbook-user.yml -kK
