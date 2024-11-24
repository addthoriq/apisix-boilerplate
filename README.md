# APISIX + APISIX DASHBOARD BOILERPLATE
## Requirement
1. Docker 27.3.1
1. docker-compose or Docker Desktop 4.36.0
## Account
1. Admin
    - username: admin
    - password: 123
1. User
    - username: user
    - password: 123
## Installation
Clone this repo
```
git clone https://github.com/addthoriq/apisix-boilerplate.git 
cd apisix-boilerplate/
```
## Usage
### Build the docker
- docker-compose
```
docker-compose up -d --build
```
- Docker Compose via Docker Desktop
```
docker compose up -d --build
```
### Check APISIX is run?
```
docker compose ps
```
or
```
docker-compose ps
```
### Stop the APISIX
```
docker compose down
```
or
```
docker-compose down
```
## Config
To modify the authentication, please go to `dashboard_conf/conf.yaml` and jump to `authentication:` on line 38
```
...
  users:                # yamllint enable rule:comments-indentation
    - username: admin   # username and password for login `manager api`
      password: 123
    - username: user
      password: 123
...
```

