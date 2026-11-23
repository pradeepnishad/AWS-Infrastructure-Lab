# Security Groups and IAM

## Windows-Server-SG
- Inbound: TCP/3389 from `10.10.1.20/32`.
- Outbound: all traffic to `0.0.0.0/0`.

## Windows-Client-SG
- Inbound: all ICMP IPv4 from `10.10.1.0/24`.
- Outbound: all traffic to `0.0.0.0/0`.

The successful ping tests prove both directions were reachable during testing. The earlier server security-group screenshot displayed only the RDP rule, so review the current rule set if recreating the lab.

## IAM
`Windows-Lab-EC2-Role` trusts the EC2 service (`ec2.amazonaws.com`) to assume the role and has the AWS-managed `AmazonSSMManagedInstanceCore` policy attached. The role is assigned to both EC2 instances.
