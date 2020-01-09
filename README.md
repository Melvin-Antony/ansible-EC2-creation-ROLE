Role Name
=========

This role can be used to deploy 2 EC2s on Ubuntu. This can be called within another playbook for faster deploying of EC2s.
 - Features:
    - Fully configurable and compatible with AWS
    - Flexible and feature rich with easy customization of roles
    - Can be modified to support additional modules
    
Requirements
------------

- Install Ansible on an ec2 Instance and setup it as Ansible-master
- Python boto library
- Create an IAM Role with Policy AmazonEC2FullAccess and attach it to the Ansible master instance (optional as the secret key and access key can be added in the vars/main.yml)

Role Variables
--------------

- Variables
```
aws_access_key: aws accesskey
aws_secret_key: aws secret key
region: us-east-2           # Change the region according to your requirement
instance_type: t2.micro     # Change the instance type according to your requirement
ami: ami-0d5d9d301c853a04a  # Change it to your need(Currently using Ubuntu)
keypair: new-server
```
