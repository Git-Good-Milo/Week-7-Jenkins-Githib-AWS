# How to set up a VCP

This readme will document how to set up a VCP on AWS and will go over CI/CD

VPC stands for Virtual Private Cloud. It can be used to house public and private sub networks where access to each netwrok can be determined through specific ip addresses and ports.
To create a VPC on AWS:

1. Select the VCP tab in Services on AWS
  - Click on Create VPC
  - Fill in name, IPv4 CIDR block
  - e.g my-first-vpc, 20.20.0.0/16
  - CIDR allows us to have multiple networks connected to the same ip address.
  - Click create

2. Select the Subnet Tab next. Subnet stands for subnetwork and they house various instances you can create on EC2. Public ones have access to the internet through the VPC, while private ones can only connect through to the public.
  - Click Create Subnet
  - Fill in the name of your subnet. Make sure to utilise good naming convention. If you have a lot of subnets you need yo be able to differentiate between them. Specifcy which ones you want public or private.
  - Select the vpc you just created
  - Select the Availability zone you want eg eu-west-1a
  - Fill in the IPv4 CIDR block using the same convention used for the VPC connected to the subnet. eg, 20.20.20.0/24
  - Click create

3. Select the Route Tables tab
  - Click create route table
  - Fill in the name tag, again paying close attention to naming convention.
  - Select the VPC you want to associate with it
  - Click Create.
  -
