## Preview


# Cart Endava

## Instalation (linux)
```sh
sudo apt install postgresql                                        # Download  PostgreSQL
git clone https://github.com/gabrielgiri/carrito-endava.git        # Clone the repo
cd carrito-endava                                                  # Move to the local repository 
npm install                                                        # download the dependencies about back (express y sequelize)
( cd public ; ../node_modules/.bin/bower install )                 # download the dependencies to the  front (angular)
node rebuild_tables.js                                             # Create the DM structure 
node load_fixtures.js                                              # Load data 
node server.js                                                     # inicializate the app
```

## Instalation  (windows)
```sh
https://www.postgresql.org/                                       # Download and install  PostgreSQL
git clone https://github.com/gabrielgiri/carrito-endava.git       # Clone the  repo
cd carrito-endava                                                 # Move to the local repository 
npm install                                                       # Install dependencies to the  back
npm express                                                       # Install  express
npm sequelize                                                     # Install  sequelize
cd public/node_modules/.bin                                       # Move to the file where you install bower
bower install                                                     # Install bower package 

In the config.json modify the following values 
{
  "db": {
    "username": "postgres",
    "password": "endava",
    "database": "postgres",
    "host": "127.0.0.1",
    "dialect": "postgres"
  }
}

node rebuild_tables.js                                            # create the db structure 
node load_fixtures.js                                             # Load the data into DB 
node server.js                                                    # Inicilaize the  app



```
