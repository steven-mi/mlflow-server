# MLFlow Server

MLFlow-server is a docker application to run an MLFlow-server on your computer. The authentication is activated by nginx. To run mlflow-server you only need Docker, Docker-Compose and an .env file with your login data.

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
## TODO
- The MLFlow app can only be accessed with authentification but requests seems not to be working
