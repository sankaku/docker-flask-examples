FROM python:3.7-alpine
RUN mkdir /flask
WORKDIR /flask

COPY ./requirements.txt /flask/
RUN pip install -r /flask/requirements.txt

COPY ./hello.py /flask/
CMD FLASK_APP=/flask/hello.py flask run --host=0.0.0.0
