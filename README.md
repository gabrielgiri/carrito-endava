# CART ENDAVA

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

# Instalation  (windows)

Download and install  PostgreSQL
See instructions below
```sh
https://www.postgresql.org/
```
### Clone the  repo
```sh
git clone https://github.com/gabrielgiri/cart-endava.git
```
### Move to the local repository 
```sh
cd cart-endava												
```
#### Ensure you have already installed nodeJs & npm:
```sh
node -v
npm -v
```

#### If not, download and install nodejs
```sh
https://nodejs.org/es/download/
```
### Install dependencies to the back-end
```sh
npm install 
```
### Install express
```sh
npm install express
```
### Install sequelize	
```sh
npm install sequelize
```
### Move to the /node_modules/.bin folder and install bower	
```sh
cd node_modules/.bin
npm install bower
```
### Install bower package 
cd .. 
cd .. 
cd public 
on /public folder
```sh
bower Install									
```
In the config.json modify the following fields with the data already setted on PostgreSQL
```sh
{
  "db": {
    "username": "postgres",
    "password": "endava",
    "database": "postgres",
    "host": "127.0.0.1",
    "dialect": "postgres"
  }
}
```
### create the db structure (on root folter)
```sh
node rebuild_tables.js  
```
### Load the data into DB  (on root folter)
```sh
node load_fixtures.js   
```
### Initiliaze the app
```sh
node server.js                                                   
```



# Instalation PostgreSQL (for windows)
- https://www.postgresql.org
![Step 1](images/instalation/postgresql-step-1.jpg)
- Download the installer
![Step 2](images/instalation/postgresql-step-2.jpg)
- Select the latest version for windows x86-64
![Step 3](images/instalation/postgresql-step-3.jpg)
- Select a folder to install PostgreSQL (Recommended default)
![Step 4](images/instalation/postgresql-step-4.jpg)
- Select all component items
![Step 5](images/instalation/postgresql-step-5.jpg)
- Enter a superuser DB password (you'll need it later)
![Step 6](images/instalation/postgresql-step-6.jpg)
- Select a port number for the server (Recommended default)
![Step 7](images/instalation/postgresql-step-7.jpg)
- Unselect checkbox stack builder (unless you need it)
![Step 8](images/instalation/postgresql-step-8.jpg)


