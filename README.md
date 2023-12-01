provider.tf - consists of AWS provider information and region
network resources.tf - consists of information about VPC, Subnets, Route Tables, AutoScaling group, Load Balancer, Internet Gateway and NAT Gateway
security resources.tf - consists of information about Security groups
ec2 resources.tf -  consists of information about EC2 instances and install of required packages
database resources.tf - RDS database configuration information

In AWS Architecture 
- EC2 instances in Autoscaling group
- VPC with Public and private subnets
- RDS for Mysql database
- Security group for incoming apache requests, mysql port and ssh port
- Load Balancer for distribution of requests
- Steps for initialize terraform scripts
  terraform init
  terraform plan
  terraform apply
- Cost saving has been designed for t2 micro instances as we have no information particular requests or load
- If it will be long term project, then we can make use of Reserved Instances depending upon the estimated load
