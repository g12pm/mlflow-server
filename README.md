# mlflow-server
Deploy mlflow with docker-compose

## Requirements
* Docker and docker-compose
* apache2-utils(ubuntu)

## Deploy
### 1. Create .env file
Environment:
* POSTGRES_USER
* POSTGRES_PASSWORD
* AWS_STORAGE_BUCKET
* AWS_ACCESS_KEY_ID
* AWS_SECRET_ACCESS_KEY
* AWS_DEFAULT_REGION

### 2. Create htpasswd
```sh
htpasswd -c .htpasswd <username>
```

### 3. Build and deploy
```sh
docker-compose build
docker-compose up -d
```

## Usage(client)
TODO