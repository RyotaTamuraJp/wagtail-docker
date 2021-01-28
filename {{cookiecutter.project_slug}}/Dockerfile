FROM python:3.7-buster

COPY ./app /app

WORKDIR /app

RUN apt update && \
    pip install --upgrade pip && \
    pip install -r requirements.txt

# CMD ["./scripts/start.sh"]