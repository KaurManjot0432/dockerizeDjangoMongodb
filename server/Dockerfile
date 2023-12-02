# Dockerfile

# Use an official Python runtime as a parent image
FROM python:3.8

WORKDIR /home/hp/Documents/dockerizeDjangoMongodb/server

COPY . .

RUN pip install -r requirements.txt

EXPOSE 8000

# Run app.py when the container launches
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "server.wsgi:application"]
