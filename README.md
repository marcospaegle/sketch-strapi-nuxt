# Installation
1) Download the repo and delete the .git folder
2) RUN: docker run -it -v $(pwd)/strapi-api:/strapi -w /strapi node:12.18.0-stretch bash -c 'cp .env.example .env && yarn install' && docker run -it -v $(pwd)/website:/website -w /website node:12.18.0-stretch bash -c 'cp .env.example .env && yarn install'

# Start UP
- docker-compose up

# Links
- strapi: http://localhost:1337
- website: http://localhost:3000
- phpMyAdmin: http://localhost:8080

# Strapi User
- User: admin
- Pass: password

# Database
- Database name: application
- User: admin
- Pass: password

# How to add a new package in NuxtJS
- docker exec -it container_name bash -c "yarn add package_name"

# Useful commands
- docker ps: see what containers are running

# Stack
- node 12.16.0
- mysql 5.7
- strapi ?
- nuxt ?
