This Fullstack Web Application uses Springboot to communicate with AWS, Postgres Images on Docker as a database, React for the frontend and Node.JS for the networking

Setup:
1> Setup the Docker Postgres Image and create a database within postgres
The following:
Composes a docker image from the docker-compose.yml file
Brings you into the shell terminal of the postgres docker image
Creates a Database named customer
```
docker compose up -d
docker exec -it postgres sh
CREATE DATABASE customer;
```
Now you can run Main.java, which will give a username to login. The password is: password (testing purposes)

2> Make sure dependencies are compatible 
- Parts may fail if dependencies are outdated

3> Run Frontend
```
cd frontend/react
npm run dev
```
Now use the username you got from step 1, password is password and you are all set
