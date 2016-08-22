# ansible-tower-rh-nfvpe-demo
Installs an Ansible Tower VM and configures it for Red Hat's OPNFV Summit 2016 Demo

Example execution:
ansible-playbook -i hosts site.yml -e aws_private_key_file=/home/abays/xxxxxx.pem -e aws_access_key=xxxxxx -e aws_secret_key=xxxxxx -e os_admin_password=xxxxxx -e os_private_key_file=xxxxxx -e os_auth_url=http://172.16.2.5:5000
