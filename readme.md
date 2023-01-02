
To use this playbook, you will need to have the following things set up:


Firstly, when you have to create an IAM role to use with EC2. Once role is created, attach it to your EC2 instance. Actions --> Security --> Modify IAM Role , select the role you created. You can use "AdministratorAccess" policy for this task. 

1-) Install Ansible on your local machine. ###apt install ansible -y

2-) Configure your AWS access keys as environment variables or in a configuration file.

3-) Install the boto Python library, which is required for the ec2_vpc_net module. ###sudo apt install python3-boto3 -y

When you complete these steps, you can test if ansible is working with the test-aws.yml file.

* vars folder contains the vars files required for ansible playbook to play.

vpc_setup.yml playbook contains;

* VPC Play
* Subnets Play
* Internet Gateway & Public Route Table
* NAT Gateway & Private Route Table
* Bastion Host Setup


