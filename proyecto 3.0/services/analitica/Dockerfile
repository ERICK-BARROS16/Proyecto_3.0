FROM python:3.9.16

WORKDIR /app

RUN apt-get update

RUN apt -y install python3-aiohttp

RUN pip install influxdb-client==1.36

RUN pip install pika==1.3.1

RUN pip install pytz

COPY services/analitica/main.py /app/main.py

CMD [ "python", "/app/main.py"]

