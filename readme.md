# 🐳 Docker NGINX - PHP - Node - MYSQl - PHPMyAdmin in Docker

## 🔍 About this
Basic configuration for a docker project based on NGINX webserver with PHP, NODE, MySQL and PHPMyAdmin.

## 📋 Images 
- PHP 8.3
- Node (LTS)
- MySQL 9.2.0
- PHPMyAdmin 5.2.2

## 🚀 Installation
Launch the following command in your terminal while inside any folder:

```bash
git clone https://github.com/lordmorphus/nginx-docker-allin-template.git .
```

While docker is launched, type the following command inside the cloned project folder:

```bash
docker-compose up -d
```

## ⚙️ Configuration

PHP user settings

```bash
📁 php/
  └── 🐳 Dockerfile     
```

NGINX user settings

```bash
📁 nginx/
  └── 🐳 Dockerfile     
```

.env & MySQL credentials settings

```bash
📁 project/
  └── ⚙️ .env     
```

## ⚙️ Useful commands

Node in container

```bash
docker-compose exec node
```

Composer in container

```bash
docker-compose exec php
```

Clean up docker-cache

```bash
docker builder prune
```

Remove docker container & images

```bash
docker rm -f $(docker ps -a -q)
docker rmi -f $(docker images -q)
```


