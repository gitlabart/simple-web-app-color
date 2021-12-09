FROM ubuntu

RUN apt-get update
RUN apt-get install -y python3 
RUN apt-get install -y python3-pip
RUN apt-get install -y curl

RUN pip install flask
RUN pip install flask-mysql

COPY . /opt/app.py

ENTRYPOINT FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port=8080

ENV APP_COLOR=pink

