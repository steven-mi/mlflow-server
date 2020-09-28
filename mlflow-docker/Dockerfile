FROM python:3.6

RUN pip install --upgrade pip setuptools \
    && pip install mlflow

WORKDIR /mlruns

EXPOSE 5000

ENTRYPOINT mlflow server --backend-store-uri sqlite:///mlflow.d --default-artifact-root /mlruns
