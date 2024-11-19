FROM ubuntu:latest
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install --break-system-packages flask
COPY api.py /app/api.py
WORKDIR /app
EXPOSE 5252
CMD python3 api.py