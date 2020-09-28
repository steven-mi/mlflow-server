# Simple Heroku MLFlow Server

This repository contains all you need to run a MLFlow server on heroku or on your local server. All you need is a .env file with your credentials and a server with docker and docker-compose.

## Getting Started
Git clone:
```
git clone
cd
```

Create a .env file with settings:

```
MLFLOW_TRACKING_USERNAME=user
MLFLOW_TRACKING_PASSWORD=pass
```

## Start locally with docker
Start container:
```
docker-compose
```

## Deploy on Heroku

```

```

## Notes
If you are using Heroku Free dynos, they will go to sleep after inactivity, and then wake up again. Thus when the mlflow client connects the app may be sleeping, causing a the communication timeout and failing the ML pipeline. If using this in automated workflows, it may be smart to wakeup the server a bit in advance by making an HTTP request to it:
```
ping ...
```
or

```
curl ...
```
