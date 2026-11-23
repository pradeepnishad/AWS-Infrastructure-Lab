# VPC and Networking

## VPC
`Windows-Lab-VPC`, CIDR `10.10.0.0/16`. DNS resolution and DNS hostnames are enabled.

## Subnet
`Windows-Lab-Subnet`, CIDR `10.10.1.0/24`, Availability Zone `ap-south-1a`. Auto-assign public IPv4 is enabled.

## Internet Gateway and route table
`Windows-Lab-IGW` is attached to the VPC. `Windows-Lab-RT` is explicitly associated with the subnet and contains:
- `10.10.0.0/16` → `local`
- `0.0.0.0/0` → Internet Gateway

Both EC2 instances use private addresses in the same subnet: SERVER01 `10.10.1.10`, CLIENT01 `10.10.1.20`.
