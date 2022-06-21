# Three-tier-web-app-in-AWS-with-VPC-ALB-EC2-RDS

***AWS network architecture***

![Screenshot from 2022-06-21 08-37-41](https://user-images.githubusercontent.com/59678465/174800812-605c2216-deee-4f41-82cd-27b79d7796bb.png)



Create a custom VPC with
3 availability zones, 
3 public subnet for web
3 private subnet for app
3 private subnet for db
Internet Gateway for public connection
3 NAT Gateways in the public subnet for the outgoin internet connection for private subnet
3 corresponding Route tables for the above

![1](https://user-images.githubusercontent.com/59678465/174800615-3a41d5cf-d79e-400e-8081-e2c184feda89.png)

