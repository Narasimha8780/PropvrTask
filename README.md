# PropvrTask

In this task, we will create an EC2 instance on AWS and deploy a containerized web application to it. The web application will be served using Docker, and we will ensure suitable security measures, including the creation of security groups to restrict network traffic.


We will utilize Terraform to set up an EC2 instance on AWS.
The instance will be started on a public subnet to ensure accessibility.
We will choose an instance type is t2.micro and os is ubuntu.
We are using the apt module(in amazon linux we use yum). 
Additional setup activities can be handled using configuration management technologies user data scripts.

In user data script we mentioned all the commands to install docker and setup MongoDB. 


We'll create a security group for the EC2 instance to control inbound and outbound traffic.
Inbound rules will allow HTTP traffic on port 80 for the web application, SSH access restricted to specific IPs for security, and the necessary port for MongoDB (default 27017) with access limited to the EC2 instance only.
