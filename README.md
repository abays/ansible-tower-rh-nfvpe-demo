# ansible-tower-rh-nfvpe-demo
Installs an Ansible Tower VM and configures it for Red Hat's OPNFV Summit 2016 Demo

Example execution:

ansible-playbook -i hosts site.yml -e aws_private_key_file=/home/abays/xxxxxx.pem -e aws_access_key=xxxxxx -e aws_secret_key=xxxxxx -e os_admin_password=xxxxxx -e os_private_key_file=xxxxxx -e os_auth_url=http://172.16.2.5:5000 -e vm_overcloud_bridge=xxxxxx -e vm_overcloud_ip=xxxxxx -e use_ansible_source=xxxxxx

Arguments:

aws_private_key_file: Location of private key file that grants SSH access to AWS VM

aws_access_key: Access key identifier for AWS account

aws_secret_key: Secret key identifier for AWS account

os_admin_password: Admin password for OpenStack overcloud

os_private_key_file: Location of private key file that grants access to OS VMs

os_auth_url: Authentication URL for OpenStack overcloud

vm_overcloud_bridge: Bridge VM will connect to in order to access OpenStack overcloud

vm_overcloud_ip: IP to be given to VM interface that connects to vm_overcloud_bridge

use_ansible_source: Clone and install Ansible from GitHub as opposed to installing through Yum (during Ansible Tower installation on VM)
