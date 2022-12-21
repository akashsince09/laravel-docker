# laravel-docker
I have created a Docker Compose File that will create a laravel app from the Dockerfile in the root of this Project repo. This Laravel app is hosted on nginx web server which has mysql as a Database server and i have also setup PhpMyAdmin so that developer will get the GUI of database.
This docker-compose.yml file will create 4 microservices
Services:-
1. App :- This will create laravel app.
2. Nginx :- This will host laravel app.
3. MySql :- This will be used as Database for the Laravel app.
4. PhpMyAdmin :- This will create the GUI of database.

We’ll need to create the docker-compose.yml file that will define the containerized environment. In this file, you’ll set up a service named app to be used by laravel. You need to know your user and uid arguments cause it will be used in the Dockerfile at build time because you’ll need permisions in directory without a root user (good practices and more safety).

You can find your USER and UID by using following commands:

$ echo $USER

$ echo $UID

And replace it with your user and uid in docker compose file.
