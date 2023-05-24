FROM python:3.7-alpine
WORKDIR /code

RUN apk add --no-cache gcc musl-dev linux-headers g++

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

# Bootstrap Opentelemetry Auto Instrumentation here

EXPOSE 5002

COPY . .
CMD ["python", "./server.py"]
