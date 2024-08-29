FROM ubuntu:latest

WORKDIR /app

COPY . .

EXPOSE 5252

RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y python3 python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED && \
    pip3 install flask 

CMD ["python3", "api.py"]
