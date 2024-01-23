# this sets up the container with python 3.11
FROM python:3.11-slim

# this copies everything in the Dockerfile directory to /app directory in the container
COPY . /app

# changing the working directory
WORKDIR /app

# installing the dependencies
RUN pip install -r requirements.txt

# exposing port 80
EXPOSE 80

# command to run
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]