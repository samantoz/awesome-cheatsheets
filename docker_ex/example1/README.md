# Dockerize a simple Python script with third-party modules

## 1. Build the Docker image

```console
docker build -t python-imdb-image .
```

## 2. Run the Docker image

Without user input:

```console
docker run -d  -name python-imdb-container python-imdb-image
```

If you want user input (comment out the `break` in [main.py](./main.py)):

```console
docker run -t -i --name python-imdb-container python-imdb-image
```
-i: interactive, -t: pseudo terminal
## 3. Stopping the container and removing the image

```console
docker stop python-imdb && docker rm python-imdb
```