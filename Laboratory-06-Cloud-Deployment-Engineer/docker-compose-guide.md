# Docker Compose Guide

## The docker-compose.yml File

```yaml
services:
  app:
    image: php:8.2-apache
    ports:
      - "8080:80"
    volumes:
      - ./app:/var/www/html
    environment:
      MYSQL_HOST: db
      MYSQL_DATABASE: student_db
      MYSQL_USER: student
      MYSQL_PASSWORD: student123
    depends_on:
      - db

  db:
    image: mysql:8.0
    environment:
      MYSQL_ROOT_PASSWORD: root123
      MYSQL_DATABASE: student_db
      MYSQL_USER: student
      MYSQL_PASSWORD: student123
    volumes:
      - db_data:/var/lib/mysql

volumes:
  db_data:
```

## What does the `services:` block do?

The `services:` block defines the containers that we want to run in Docker Compose. In our setup, we have two services, the app and the database. It helps us run and manage both containers together.

## How did the app container find the database?

The app container finds the database using `MYSQL_HOST: db`. The `db` is the name of our database service. Docker Compose allows the app and database to communicate with each other using the service name.

## docker run vs docker-compose up -d

The `docker run` command is used to create and start a container manually. We need to configure each container separately. While `docker compose up -d` allows us to start multiple containers using one YAML file, and `-d` means the containers will run in the background.

**Short Explanation:** Docker Compose makes our work easier because we can manage the application and database containers in one file instead of running them one by one.
