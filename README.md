# AWS_studyproject
**VPC with servers in private subnets and NAT**

To demonstrate to create a VPC that you can use for servers in a production environment.

To improve resiliency, you deploy the servers in two AZ’s by using Auto scaling group and an Application load balancer. For additional  security,
you deploy the server in a private subnets, The servers receive requests  through the load balancer. The servers can connect to the internet by using a NAT gateway. To improve resiliency, you deploy the NAT gateway in both AZ’s.


<img width="618" alt="image" src="https://github.com/Akash051198/AWS_studyproject/assets/63510805/536f7ec2-93f0-4061-ba93-91be9613b693">

**Overview**:

The VPC has public subnets and private subnets in the two AZ’s.

Each public subnet contains NAT gateway and a load balancer node.

The servers run in the private subnets, are launched and terminated by using an Auto Scaling group, and receive traffic from the load balancer.

The servers can connect to the internet by using a NAT gateway
