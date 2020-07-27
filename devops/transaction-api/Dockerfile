FROM python:3.6-alpine3.11
WORKDIR /transaction-api

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

EXPOSE 5000
COPY . .
CMD ["python", "run.py"]