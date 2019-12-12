# terraform-aws-demostack
    This Project configures Nomad, Vault and Consul on a variable amount of servers and workers. it already set up some nomad jobs, vault configurations and Consul queries. this is meant as a reference (and a demo enviroment) and really shouldnt be used for production. 
## Solution Diagram
![Solution Diagram](./assets/Demostack_overview.png)

## Dependencies
 <TODO>

 ### TLS

 <TODO>

 ## Consul

 <TODO>

 ## Vault

 <TODO>

 ## Nomad
 
 <TODO>


## Changes
- terraform.tfvars
  - owner: i use my name
  - primarynamespace
  - secondarynamespace
  - public_key
  - servers: default is 3. test with 1
  - workers: default is 3. test with 0 or 1
  - vaultlicense
  - consullicense
  - enterprise = default is false. true for testing enterprise features


## troubleshooting
To begin debugging, check the cloud-init output:

```shell
$ sudo tail -f /var/log/cloud-init-output.log
```