# MLFlow Server

This repository contains all you need to run a MLFlow server on your server. All you need is a .env file with your credentials and a server with docker and docker-compose.

## Getting Started
**Git clone:**
```
git clone https://github.com/NewsPipe/simple-heroku-mlflow-server.git
cd simple-heroku-mlflow-server
```

**Create a .env file with settings:**

```
MLFLOW_TRACKING_USERNAME=user
MLFLOW_TRACKING_PASSWORD=pass
```

## Start locally with docker
**Start container:**
```
docker-compose up --build
```
