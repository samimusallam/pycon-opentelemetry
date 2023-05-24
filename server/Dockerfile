FROM python:3.9-alpine3.14
WORKDIR /code

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

# Bootstrap Opentelemetry Auto Instrumentation here

EXPOSE 5002

COPY . .
CMD ["python", "./server.py"]
