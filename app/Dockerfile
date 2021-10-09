FROM python:3.6-alpine

COPY ./src /app

WORKDIR /app

RUN pip install -r requirements.txt

CMD ["python", "app.py"]

EXPOSE 5000

HEALTHCHECK  CMD curl --fail "http://localhost:8080" || kill 1
