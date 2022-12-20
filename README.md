# laravel-docker


You’ll need to create the docker-compose.yml file that will define the containerized environment. In this file, you’ll set up a service named app to be used by laravel. You need to know your user and uid arguments cause it will be used in the Dockerfile at build time because you’ll need permisions in directory without a root user (good practices and more safety).

You can find your USER and UID by using following commands:

$ echo $USER

$ echo $UID

And replace it with your user and uid in docker compose file.
