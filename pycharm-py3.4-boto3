FROM python:3.6

LABEL maintainer "Roger Gomez <rogerscuall@gmail.com>"

WORKDIR /opt/project
RUN apt-get update -y -qqqq
RUN apt-get install -y -qqqq python-pip >> /dev/null
COPY requirements.txt .
RUN pip install -r requirements.txt -q
CMD [ "/opt/pycharm/bin/pycharm.sh" ]
