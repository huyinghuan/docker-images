## How to use

- create registry store directory, and bind on `docker-compose` : `volumes`
- create certs file and bind on `docker-compose` : `volumes`
- modify  `docker-compose` bind yourself ip
- nginx config: `nginx.conf`


## How to create certs

`openssl req -newkey rsa:4096 -nodes -sha256 -keyout auth.key -x509 -days 365 -out auth.crt`

## GITHUB
- https://hub.docker.com/_/registry/
- https://github.com/huyinghuan/docker_auth
- https://github.com/huyinghuan/docker-registry-frontend