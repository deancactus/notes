# Notes
Markdown notes are pretty. Pretty notes are easier to read.

## Project Ideas
1. TeX resume

   Build it in docker
   [Example](https://github.com/maciaszczykm/resume "TeX Resume Example")
1. Python examples
1. Kubernetes bits
1. Salt formulas
1. AWS cert

## Docker

*  There's no built-in support in Docker Desktop Win/Mac for remote 'hosts' access

   You can run a container to expose a port for this purpose:
   [private/insecure](https://hub.docker.com/r/jarkt/docker-remote-api)
   or [with tls](https://hub.docker.com/r/kekru/docker-remote-api-tls)

   Configure remote clients with -H option on the command line or DOCKER_HOST environment variable

*  There is a chocolately package for installing just the
   [docker-cli](https://chocolatey.org/packages/docker-cli) on Windows

   It seems to work just fine with the Docker VSCode extension

## Terraform
### Bastion + WebServers
1. Have the bastion assume a role (with ec2, route53)
1. Augment the output to return all the IPs
1. Augment the dns record to include all the EIPs

### Moving forward
1. Separate the bastion creation into its own project?
1. Chain the terraform s/t most of the resources are created/managed from the bastion?
1. Run ansible/salt/other from the bastion to configure basic webservers
1. Set up additional resources for WordPress (ALB, MySQL/Aurora DB, CloudFront, S3)


## AWS
1. Read up on ALB

## Salt
*  If `pillar.items` shows your data but `pillar.items key` doesn't, there may an issue with the formatting of the data.