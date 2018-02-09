Library app is education project developing by [savecart](https://savecart.pl/) team.

#### Project requirements

- node-carbon (v. 8.9.4)
- [docker](https://docs.docker.com/install/) & [docker-compose](https://docs.docker.com/compose/install/)

#### Installation
Application use express.js and mongoDB docker containers. You must to install all node packages. In __**main directory**__ run command.

`$ npm install`

Next step is run docker containers.

`$ docker-compose up -d`

You can  chek for everything is correct. 

`$ docker ps`

correct output is: 

```
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS                      NAMES
382052e4e843        library_web         "npm start"              About an hour ago   Up About an hour    0.0.0.0:49160->8080/tcp    library_web_1
64ada740abb9        mongo               "`docker-entrypoint.s…"   About an hour ago   Up About an hour    0.0.0.0:27017->27017/tcp   library_mongo_1

```

When express.js and mongoDB is running, you need start vue.js application. Open __**application**__ folder and install required packages.

`$ npm install`

Then you can start app.

`$ npm run dev`

App will be available on:

`localhost:8080`

#### Running app

Start docker containers. Run command in __**main**__ folder. 

`$ docker-compose up -d`

Start vue app. Run command in __**application**__ folder.

`$ npm run dev`

App will be available on:

`localhost:8080`

MongoDB connection

`$ mongo 127.0.0.1:27017/budgetmanager`


