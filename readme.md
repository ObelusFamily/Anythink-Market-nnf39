# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_
**[Updated on 14/08/2022 Instructions on how to run the docker container]**


1. Installing docker
First things first, we need install docker. You can view the instructions here https://docs.docker.com/get-docker/.

Great!You can verify docker is ready by running the following commands in your terminal: docker -v and docker-compose -v.


2. Running the container for the project

Then, from the project repository, run docker-compose up, to set up both the frontend and the backend.

If the container was setup correctly, the backend should be running and able to connect to your local database.

To confirm that, point your browser to http://localhost:3000/api/ping
It should show a message saying that you are ready to go!


3. Setup an user
After that, it's time to create a user for yourself inside the container (this if proof that the frontend is connected to the backend).

Go to http://localhost:3001/register and create a user, password and email.


4. All set to go nowhere.

Now all you have to do from now on is to run all scripts inside one of the containers created by "docker-compose up".
Remember, you can use "docker exec" to run commands on a running container.


