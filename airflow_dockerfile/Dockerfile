FROM apache/airflow:2.10.5-python3.9

COPY req.txt /req.txt

RUN python -m pip install --upgrade pip && \
    pip install --no-cache-dir -r /req.txt

USER root
RUN apt update && \
    apt install -y openjdk-17-jdk

USER airflow