# Rails 5 docker image

This image allows you to easily develop Rails 5 app.
As Rails version 5 is still in beta, you need a custom image
to be able to use it.


## Details

Currently the image uses Rails 5 beta 3 riding Ruby 2.3.0. It will be
updated over time to always use the edge version of Rails and latest
version of Ruby.


## How to use it

### Option 1
You can build the image straight from the **Dockerfile**:
```
docker build .
```

### Option 2
You can run it individually from your project's root folder:
```
docker run -it -v $(pwd):/app bartoffw/rails5
```

### Option 3
Or you can use [Docker Compose](https://docs.docker.com/compose/overview/) to run the entire environment:
```
docker-compose up
```
Before running Docker Compose you need to place the `docker-compose.yml` file
in your project's root folder. No need to copy any other files.


## Plans

My nearest future plans are to include some other images to make a full
development environment ready for use.


# License

MIT
