# EC2 and EBS

## EC2
Both instances are shown running in `ap-south-1a`:
- SERVER01: Windows Server 2025 Datacenter, `c7i-flex.large`, private IPv4 `10.10.1.10`, IMDSv2 required.
- CLIENT01: Windows Server 2025 Datacenter, `c7i-flex.large`, private IPv4 `10.10.1.20`, IMDSv2 required.

Each instance type is shown with 2 vCPU and 4 GiB memory. Public IPv4 addresses have been omitted from this report because auto-assigned addresses can change.

## EBS root volumes
Both root volumes are 40 GiB gp3, with 3,000 IOPS and 125 MiB/s throughput. Encryption is enabled using the AWS-managed KMS key alias `aws/ebs`. Both volumes are in-use, status check Okay, initialization Completed, and Multi-Attach disabled.
