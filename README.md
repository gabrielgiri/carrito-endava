## Preview

![Carrito Endava Preview](images/carrito.jpg)

## Instalation (linux)
```sh
sudo apt install postgresql                                        # Download  PostgreSQL
git clone https://github.com/gabrielgiri/cart-endava.git           # Clone the repo
cd cart-endava                                                     # Move to the local repository 
npm install                                                        # download the dependencies about back (express y sequelize)
( cd public ; ../node_modules/.bin/bower install )                 # download the dependencies to the  front (angular)
node rebuild_tables.js                                             # Create the DM structure 
node load_fixtures.js                                              # Load data 
node server.js                                                     # inicializate the app
```

## Instalation  (windows)
```sh
https://www.postgresql.org/									# Download and install  PostgreSQL
git clone https://github.com/gabrielgiri/cart-endava.github	# Clone the  repo
cd cart-endava												# Move to the local repository 

	Ensure you have already installed nodeJs & npm:
node -v
	You must see something like:
v6.10.3

npm -v
	You must see something like:
6.1.0

	If not install nodejs 									# Install NodeJs
https://nodejs.org/es/download/

npm Install 												# Install dependencies to the back-end
npm express													# Install express
npm sequelize												# Install sequelize
cd public/node_modules/.bin									# Move to the file where you install bower
bower Install 												# Install bower package 

In the config.json modify the following fields with the data already setted on PostgreSQL
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
