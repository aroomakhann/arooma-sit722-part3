# Dockerfile for inventory-management microservice

FROM --platform=linux/amd64 python:3.11-slim

WORKDIR /app

COPY ./requirements.txt /app/requirements.txt

COPY ./app /app/app

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 3002

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "3002"]
