# fos-test

This is a test project created to provision a VM on AWS and deploy 3 containers

To provision the VM on AWS:

ansible-playbook /vagrant/Ansible/provision-aws/sites.yml

This playbook needs to have installed and configured boto: 

$ pip install -U boto
$ cat ~/.boto
[Credentials]
aws_access_key_id = YOUR_AWS_ACCESS_KEY_ID
aws_secret_access_key = YOUR_AWS_SECRET_KEY

To configure and deploy the containers:

ansible-playbook /vagrant/Ansible/configuration/sites.yml

