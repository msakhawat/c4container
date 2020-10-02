FROM ubuntu:20.04

# RUN apt-get update && apt-get -y install python3 && apt-get -y install python3-pip

####for dev purpose
RUN apt-get update
RUN apt-get -y install python3 && apt-get -y install python3-pip

RUN pip3 install flask flask-mysql
#########
COPY ./src .
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
EXPOSE 5000

CMD ["flask", "run"]
