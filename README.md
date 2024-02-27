# nginx_proxy
dockerized nginx reverse proxy

## Summary
Sets up an nginx load labancer / reverse proxy that serves 2 Docker container webapps
- Load Balancer
- Reverse Proxy

NOTE: the intent of this small project is to provide a minimalistic & easily incorporable module to use in a larger project

## Requirements
- Docker & docker-compose
- open web ports (80)

## Set Up
- docker-compose up -d

## Use
- run [Set Up](#set-up)
- curl localhost
	- forwards traffic to upstream frontend, which is our load balancer switching between server1 & server2
- curl app1.localhost
  - loads docker container for server1
- curl app2.localhost
  - loads docker container for server2

## Troubleshooting
- Error:
  - Cause:
  - Remediation:

## Notes
- venv used to execute pre-commit hooks
  - ```shell
    & "C:\Python311\python.exe" -m venv venv
    .\venv\Scripts\activate
    python -m pip install --upgrade pip
    pip install logging logger openai nltk boto3 awscli
    ```
- misc

## TODO
- incorporate https / ssl certs

## References
- http://jasonwilder.com/blog/2014/03/25/automated-nginx-reverse-proxy-for-docker/
- https://www.toptal.com/developers/gitignore
