FROM python:3.6-alpine3.11

WORKDIR /loyalty-worker

ENV HTTP_PORT=5000
ENV REDIS_URL=redis://127.0.0.1:6379/0

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
EXPOSE 5000

COPY . .
CMD ["python", "run.py"]