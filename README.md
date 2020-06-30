# PHPBB 3.3.x Styles

A development setup for PHPBB 3.3.x styles. Please view the [phpbb styles docs](https://www.phpbb.com/styles/create/) for more instructions on how to set up a new style.

## Pre-Requisites

- [Docker](https://docs.docker.com/get-docker/)

## Use

1. In your terminal, navigate inside this folder. [If you've never used the terminal before, this may help!](https://openclassrooms.com/en/courses/4614926-learn-the-command-line-in-terminal/4634356-navigate-your-system)
2. If you're creating a new style:
   - Copy the "prosilver" folder inside of this folder/repository. Each folder in this folder/repository will appear as a style after launching the system.
   - Rename the folder to your style name, and update the style.cfg file.
3. Type `docker-compose up`
4. You may access your local instance of phpbb and phpadmin (the database) via the browser.
   - To access the forums, naviate to `localhost` in your browser.
     - The default admin login:
       - username: user
       - password: bitnami
   - To access phpadmin, navigate to `localhost:8080`
     - username: root
     - no password (leave this box blank)
5. Start creating!
   - I reccomend having two tabs open--the [admin console](http://localhost/adm/index.php), to clear the cache, and whatever page you're working on.
6. To exit and clean up all the files relating to your development enviroment:
   - Hit `control c` in your terminal.
   - Type `docker-compose down` if you'd like to keep around the database when developing in the future. Type `docker-compose down -v` if you'd also like to delete the docker volumes, i.e. wipe the database.
