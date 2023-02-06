# syntax=docker/dockerfile:1

FROM ubuntu:latest

WORKDIR /app

RUN apt-get update -y

RUN apt-get install -y python3-pip python3-dev build-essential hdf5-tools libgl1 libgtk2.0-dev

COPY ./requirements.txt /app/requirements.txt

RUN pip3 install -r requirements.txt
	
COPY . /app

EXPOSE 6040

CMD ["python3", "api.py"]
