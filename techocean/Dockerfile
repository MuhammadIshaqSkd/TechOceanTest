FROM python:3.8-slim-buster

ENV PYTHONUNBUFFERED 1

WORKDIR /app

ADD . /app

COPY requirement.txt /app/requirement.txt

RUN pip install -r requirement.txt

COPY  . /app

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
