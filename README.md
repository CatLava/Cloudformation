# Cloudformation template

The cloudformation template is used to spin up 4 servers per spec outlined in Udacity's assignment for cloud formation. There are two files, final.yml and params.json . The final.yml contains all the cloudformation configurations to spin up VPC, 4 subnets ( 2 private, 2 public), Internet Gateway, Nat gateways, security groups, load balancers, and a bastion host.

This script is configurable for more additions.

## Installation

To run this package from a linux based command line, ensure your aws cli tools are configured properly and run something along the lines of.
```aws cloudformation create-stack
--stack-name YOUR STACK NAME
--template-body file://final.yml
--parameters file://params.json
```

## Acknowledgements

This project was successfully created with the help of instructors at Udacity. Along with the well formatted AWS documentation and infrastructure.
