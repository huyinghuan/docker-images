## How to use
- modify `docker-compose.yaml`:  `registry`.`environment`.`REGISTRY_AUTH_TOKEN_REALM` the domain
- create registry store directory, and bind on `docker-compose` : `volumes`
- create certs file and bind on `docker-compose` : `volumes`
- nginx config: `nginx.conf`


## How to create certs

`openssl req -newkey rsa:4096 -nodes -sha256 -keyout auth.key -x509 -days 365 -out auth.crt`

## GITHUB
- https://hub.docker.com/_/registry/
- https://github.com/huyinghuan/docker_auth
- https://github.com/huyinghuan/docker-registry-frontend

## fluentd

https://docs.fluentd.org/v1.0/articles/config-file