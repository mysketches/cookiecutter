FROM python:3

ADD requirements.txt requirements.txt

RUN pip install -r requirements.txt
RUN mkdir /home/project

WORKDIR /home/project 
CMD /bin/bash