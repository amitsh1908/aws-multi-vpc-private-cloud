## Setup Summary

1. Created VPC-A and VPC-B
2. Created public and private subnets in VPC-A
3. Created private subnet in VPC-B
4. Attached IGW to VPC-A
5. Configured route tables for public and private subnets
6. Launched Bastion Host in public subnet
7. Launched App-A and App-B in private subnets
8. Created NAT Gateway with Elastic IP
9. Updated private route table to use NAT
10. Created VPC Peering between VPC-A and VPC-B
11. Updated routes for private communication
12. Configured Security Groups with least privilege