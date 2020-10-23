# create_webserver_in_custom_vpc_terraform
This repo shows sample creation of a webserver in a custom subnet in your own custom VPC

**Note:** Before creating the following resources in terraform, login to your EC2 console in your AWS account and create an EC2 keypair, it would be required un step 9 below, when you're creating the EC2 instance.

The terraform code creates the following resources in your AWS account

1. Create VPC

2. Create Internet Gateway

3. Create Custom Route Table

4. Create Subnet

5. Associate subnet with Route Table

6. Create Security group to allow port 22, 80, 443

7. Create a network interface with an IP in the subnet that was created in step 4

8. Assign the Elastic IP to the network interface created in step 7

9. Create Ubuntu server and install/enable Webserver
