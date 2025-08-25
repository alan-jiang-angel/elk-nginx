# Docker Compose for ELK with Nginx

This repo is for running ElasticSearch, Logstash and Kibana with Nginx.

Logstash is configured to log all PM2 logs and Nginx is used for basic Authentication.


## Requirements

1. Install docker
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04

2. Set password for basic Authentication

```sudo apt install apache2-utils -y```

  Create password by running following command. Username is `admin`

```htpasswd -c nginx/.htpasswd admin```

3. Run docker containers

```docker compose up -d```

4. Open Kibana

Visit http://YOUR-IP
