FROM python:3.7-alpine
WORKDIR /code

RUN apk add --no-cache gcc musl-dev linux-headers g++

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

# Install OpenTelemetry Auto Instrumentation Here

EXPOSE 5000

COPY . .
CMD ["python", "./server.py"]
