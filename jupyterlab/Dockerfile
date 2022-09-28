FROM jupyter/scipy-notebook
USER root
COPY requirements.txt .
RUN apt-get update && apt-get -y install libpq-dev
RUN pip install requests feature_engine
RUN pip install -r requirements.txt && rm requirements.txt