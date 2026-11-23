# Systems Manager and Connectivity Validation

## Fleet Manager
Fleet Manager shows two managed nodes, SERVER01 and CLIENT01. Both are Running and have Ping status Online. Both report Windows Server 2025 Datacenter and SSM Agent version `3.3.5700.0`. Browser desktop session captures are included for both nodes.

## Private IP connectivity
### CLIENT01 to SERVER01
`ping 10.10.1.10`: 4 sent, 4 received, 0% loss; response times shown as less than 1 ms.

### SERVER01 to CLIENT01
`ping 10.10.1.20`: 4 sent, 4 received, 0% loss; response times shown as less than 1 ms.

These tests establish private IPv4 reachability at the time captured. They do not prove DNS name resolution or application-layer connectivity.
