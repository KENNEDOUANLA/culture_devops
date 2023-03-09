FROM python:2.7-stretch
LABEL MAINTAINER="KENNE Web developper"
RUN apt-get -y update && apt-get -y install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev && \
    pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0

RUN mkdir /data 
COPY ./  /
VOLUME [ "/data" ]
EXPOSE 5000

CMD [ "python","./student_age.py" ]