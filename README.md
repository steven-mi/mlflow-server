# Simple Heroku MLFlow Server

This repository contains all you need to run a MLFlow server on heroku or on your local server. All you need is a .env file with your credentials and a server with docker and docker-compose.

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

## Deploy on Heroku
****
```

```

## Notes
If you are using Heroku Free dynos, they will go to sleep after inactivity. Therefore when your MLFlow client tries to connect to the server, it may be sleeping. This causes a communication timeout. It is recommended to sent out a request, before your MLFlow client tries to connect.
