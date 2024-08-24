FROM python:3.12-slim 

WORKDIR / app

COPY requirements.txt .

RUN pip install -r requirements.txt --no-cache-dir

COPY . .

EXPOSE 5004

CMD ["python", "app.py"]