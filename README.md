# Docker Compose for ELK with Nginx


## Requirements

1. Install docker
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04

2. Set password for basic Authentication

```sudo apt install apache2-utils -y```

Create password by running following command. Username is `admin`
```htpasswd -c nginx/.htpasswd admin```

3. Run docker containers
```docker compose up -d```
