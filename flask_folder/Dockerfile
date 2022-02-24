FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y python3-pip python3.7
ENV PYTHONDONTRUNBYTECODE 1
ENV PYTHONBUFFERED 1

RUN mkdir /app
COPY ./myproject/ /app

WORKDIR /app
RUN pip3 install -r requirements.txt
EXPOSE 5001
CMD ["python3", "app.py"]         

