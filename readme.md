# terraform AWS VPC Module Customised

This module is going to create the following resources. For HA we are going to get first 2 AZ

* vpc
* internet gateway associated with vpc
* 2 public subnets
* 2 private subnets
* 2 database subnets
* database subnet groups
* eip
* nat gateway
* Public route table
* private route table
* database route table
* routes
* route table associations with subnets
* peering with default vpc(if required)
* peering routes in acceptor and requester route tables

# inputs
Project_name (mandatory): user must supply their project name.
environment (mandatory): user must supply environment
vpc_cidr (mandatory): user must supply vpc cidr
enable _dns_hostnames (optional): defaults to true
common_tags (optional)
vpc_tags(optional)
igw_tags(optional)
public_subnet_cidrs (mandatory)
public_subnet_tags(optional)
private_subnet_cidrs (mandatory)
private_subnet_tags(optional)
database_subnet_cidrs(mandatory)
database_subnet_tags(optional)
db_subnet_group_tags(optional)
nat_gateway_tags (optional)
public_route_table_tags(optional)
private_route_table_tags(optional)
database_route_table_tags(optional)
is_peering_required(optional)
vpc_peering_tags(optional)