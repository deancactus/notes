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