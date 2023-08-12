# pull official base image
FROM python:3.11.4-slim-buster

# set work directory
WORKDIR /usr/src/app

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
ENV PORT 8080

COPY . .

# install dependencies
RUN pip install --upgrade pip && pip install -r requirements.txt

CMD ["sh", "-c", "python manage.py runserver 0.0.0.0:$PORT"]
