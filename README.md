# Secure Multi-VPC Architecture on AWS

-This project demonstrates a secure, production-style AWS networking setup using
 multiple VPCs, private subnets, a bastion host, NAT Gateway, and VPC peering.
-This infrastructure was created manually using the AWS Console and verified
 using AWS CLI exports.

## Architecture Overview
- VPC-A
  - Public Subnet: Bastion Host
  - Private Subnet: App-A
  - Internet Gateway + NAT Gateway
- VPC-B
  - Private Subnet: App-B (no internet access)
- Secure private communication using VPC Peering

## Key Components
- Public and Private Subnet separation
- Bastion Host for controlled SSH access
- NAT Gateway for outbound internet access from private subnet
- VPC Peering for private inter-VPC communication
- Security Groups with least-privilege access

## Repository Structure
architecture/  -> Architecture diagram
exports/       -> AWS CLI exports (proof of infrastructure)
notes/         -> Step-by-step setup notes

## Proof
All infrastructure details are exported using AWS CloudShell and AWS CLI
and stored in the `exports/` directory.

## Skills Demonstrated
- AWS VPC & Subnet Design
- Route Tables & NAT Gateway
- Bastion Host Access Pattern
- VPC Peering
- CloudShell & AWS CLI
- Secure Network Design

