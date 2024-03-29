# AWS_studyproject
VPC with servers in private subnets and NAT

This demonstrate how to create a VPC that you can use for servers in a 
production environment.

To improve resiliency, you deploy the servers in two AZ’s by using Auto scaling group and an Application load balancer. For additional  security,
you deploy the server in a private subnets, The servers receive requests  through the load balancer. The servers can connect to the internet by using a NAT gateway. To improve resiliency, you deploy the NAT gateway in both AZ’s.
