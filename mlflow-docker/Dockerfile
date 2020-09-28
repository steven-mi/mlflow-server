FROM python:3.6

# install mlflow
RUN pip install --upgrade pip setuptools \
    && pip install mlflow

# set mlruns as workdir and start mlflow server
WORKDIR /mlruns
EXPOSE 5000
ENTRYPOINT mlflow server --backend-store-uri sqlite:///mlflow.d --default-artifact-root /mlruns --port 5000 --host 0.0.0.0
