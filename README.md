# Project Title

## Overview

Micro frontend for Login

## Prerequisites

- Docker
- Docker Compose

## Steps to Run Dev Server Using Docker

### 1. Create .env File

Create a `.env` file in the project root and copy the content from `.env.example`. Change the values accordingly:

```
REACT_APP_API_BASE_URL='http://localhost:3001/login'
REACT_APP_API_VERSION='v1'
REACT_APP_REDIRECT_URL='/home'

NODE_ENV=development
PORT=3001
JWT_SECRET='your_jwt_secret'
JWT_EXPIRATION_MINUTES=15
MYSQL_HOST='your_mysql_host'
MYSQL_PORT=your_mysql_port'
MYSQL_USER='your_mysql_user'
MYSQL_ROOT_PASSWORD='your_mysql_root_password'
MYSQL_DATABASE='your_mysql_database'
```

### 2. Build and Run the Docker Containers

Run the following command to build and start the Docker containers:

```sh
docker-compose -f docker-compose-dev.yml up --build
```

## Additional Information

Any additional information or instructions.
