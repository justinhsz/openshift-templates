FROM python:3.7-alpine

EXPOSE 5000

ENV FLASK_APP=/app/wsgi.py

RUN mkdir /app
COPY . /app/

RUN pip install -r /app/requirements.txt --no-cache-dir

ENTRYPOINT [ "flask", "run", "--host=0.0.0.0" ]