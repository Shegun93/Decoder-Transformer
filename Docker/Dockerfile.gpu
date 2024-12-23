FROM tensorflow/tensorflow:2.15.0-gpu

RUN apt-get update && \
    pip install --upgrade pip

WORKDIR /app

COPY ./requirements.txt /app

RUN pip install -r /app/requirements.txt

COPY ./GPT.ipynb /app
COPY /Data/. /app/Data
COPY /checkpoint/. /app/checkpoint

ENV PYTHONPATH="${PYTHONPATH}:/app"