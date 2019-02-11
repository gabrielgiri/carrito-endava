# Carrito Endava

## Instalación resumida
```sh
sudo apt install postgresql                                        # bajar PostgreSQL
git clone https://github.com/gabrielgiri/carrito-endava.git        # clonar el repo
cd Carrito                                                          # cambiar a la nueva carpeta donde vive el repo local
npm install                                        # bajar las dependencias del back (express y sequelize)
( cd public ; ../node_modules/.bin/bower install ) # bajar las dependencias del front (angular)
node rebuild_tables.js                             # armar la estructura de la BBDD
node load_fixtures.js                              # cargarla con datos
node server.js                                     # arrancar la app
```

## Instalación

### Dependencias Node (Server side)

    npm install

### Dependencias Bower (Client side)

    cd public
    bower install

### Estructura de base de datos

    node rebuild_tables.js

### Datos de prueba

    node load_fixtures.js

### Iniciar servidor

    node server.js
