# Dockerfile: Blueprint for building/creating images (base image with python in this case)
# Image: Template for running containers
# Container: Running process with the App in it

FROM python:3.9
WORKDIR /code
COPY ./requirements.txt /code/requirements.txt
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt
COPY ./app /code/app
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]