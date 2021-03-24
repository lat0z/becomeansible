# ad-hoc Ansible Commands 


```
ansible localhost -m ping

ansible localhost -m stat -a "path=/ansible"

ansible all -m ansible.builtin.setup 

ansible all -i <Public Ip Address>, -m ping -e "ansible_user=ansible ansible_password=<Password> ansible_ssh_common_args='-o StrictHostKeyChecking=no'"

ansible all -i <Public Ip Address>, -m win_ping -e "ansible_user=ansible ansible_password=<Password> ansible winrm_server_cert_validation=ignore ansible_connection=winrm"

```
