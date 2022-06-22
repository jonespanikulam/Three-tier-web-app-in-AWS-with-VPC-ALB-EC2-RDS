# Three-tier-web-app-in-AWS-with-VPC-ALB-EC2-RDS

***AWS network architecture***

![Screenshot from 2022-06-21 08-37-41](https://user-images.githubusercontent.com/59678465/174800812-605c2216-deee-4f41-82cd-27b79d7796bb.png)



Create a custom VPC with

3 availability zones, 

3 public subnet for web

3 private subnet for app

3 private subnet for db

3 route table and associate with the subnets

Internet Gateway for public connection

3 NAT Gateways in the public subnet for the outgoin internet connection for private subnet

3 corresponding Route tables for the above

![1](https://user-images.githubusercontent.com/59678465/174800615-3a41d5cf-d79e-400e-8081-e2c184feda89.png)

Summary:

Here we create jumb server, 2 application server and Rds server. Jumb server is in public subnet connected to an internet gateway
for connection. The application servers and RDS are routed using NAT gateways.

The application servers are therefore accessed using the jumb servers and we install php and https webserver. Then we create a application
load balancer and add the php servers as it targets. The round robin mechanism is present in the php servers.

We then create RDS instance and add the subent groups required. Install phpmyadmin in php servers and add the RDS endpoint in config file to connet
to the phpmyadmin. We need to add stickiness feature in ALB, otherwise the phpservers get intercoonected using round robin. 

![1](https://user-images.githubusercontent.com/59678465/175048348-08974967-d4e5-420b-b57d-6a8bc04c6629.png)





