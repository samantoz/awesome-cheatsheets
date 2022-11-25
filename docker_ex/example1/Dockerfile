# Dockerfile: Blueprint for building/creating images (base image with python in this case)
# Image: Template for running containers
# Container: Running process with the App in it

FROM python:3.9
ADD main.py .
RUN pip install requests beautifulsoup4
CMD ["python", "./main.py"]