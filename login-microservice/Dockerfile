FROM python:3.12-slim AS builder 

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt --no-cache-dir

COPY . .

EXPOSE 5003

CMD ["python", "app.py"]
