# terraform-aws-vpc

This module creates the foloowing resources.
* VPC
* IGW
* 2 Public subnets in us-east-a and us-east-b AZ
* 2 Private subnets in us-east-a and us-east-b AZ
* 2 Database subnets in us-east-a and us-east-b AZ
*  Public Route table
*  Private Route table
*  Database Route table
*  EIP for NAT
* NATGateway in public subnet a AZ
* IGW route is added to public route table
* NAT gateway route to private and database route tables
* Route table association with subnets
* VPC to default VPC peering
* Public route table to default VPC route 
* Default VPC main route table to created VPC route

### Inputs
* vpc_cidr - (Required). User must suppy the CIDR for VPC.
* project_name - (Required). User must supply the project name.