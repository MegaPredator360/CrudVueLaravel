# CRUD Basico en Laravel - Vue JS
Esta es una aplicacion web diseñada con el objetivo de aprender las tecnologias de Laravel y Vue JS.<br />
Posiblemente esta aplicacion sea reconstruida en un proyecto más complejo para poder aprender cada detalle de las funcionalidades de dichas tecnologias y expandir más mi conocimiento.

Este proyecto fue diseñado con:
- MongoDB
- Laravel (PHP)
- Vue JS

## Tabla de Contenido
* [Objetivos](#objetivos)
* [Requisitos](#requisitos)
* [Ejecución](#ejecución)
    * [API - Laravel](#api---laravel)
    * [Vue JS](#vue-js)
* [Desarrollador](#desarrollador)

## Objetivos
El objetivo de esta aplicacion es poder aprender las tecnologias de Laravel, PHP, y MongoDB. Y poder expandir mis conociemientos con estas tecnologias. Eventualmente se tiene pensando desarrollar un proyecto de Sistema de Ventas demostrando una aplicacion más compleja, pero que sirva como experiencia con estos lenguajes y tecnologias.

## Requisitos
Para la ejecución de este proyecto se necesita lo siguiente:
- Un IDE, se recomienda: [Visual Studio Code](https://code.visualstudio.com/).
- [PHP](https://www.php.net/manual/en/install.php) 8.2.20 o superior.
- [Controlador de MongoDB](https://www.mongodb.com/docs/drivers/php-drivers/) para PHP.
- [Node JS](https://nodejs.org/en).
- [MongoDB Community Edition](https://www.mongodb.com/docs/manual/installation/).

## Ejecución
### API - Laravel

- Una vez instalados los programas requeridos, clonas este repositorio y lo guardas en la carpeta de tu preferencia. Si utilizas la aplicacion de consola **git**, podrás clonar el proyecto con el siguiente comando:
```console
git clone https://github.com/MegaPredator360/CrudVueLaravel.git
```
- Una vez que hayas clonado el proyecto serás presentado con 2 carpetas:
    - **CrudApiLaravel:** Esta carpeta contiene los archivos de la aplicacion de Laravel, escrito en PHP.
    - **CrudVue:** Esta carpeta contiene los archivos de la aplicacion de Vue JS.

- Para configurar la API, tenemos que instalar las dependencias del proyecto, por lo tanto, se abre una consola en la carpeta de **CrudApiLaravel** y se ejecuta el siguiente comando:
```console
composer install
```
- Despues puede configurar la conexion hacia tu base de datos, por defecto, ya tiene una conexion de forma local hacia la aplicacion de Laravel, sin embargo, si desea modificar la conexion a la base de datos de MongoDB, dirigite al archivo `config/database.php`, y encontrarás un codigo como este:
```
'mongodb' => [
    'driver' => 'mongodb',
    'dsn' => env('DB_URI', 'mongodb://localhost:27017'),
    'database' => 'CrudDB'
]
```

- Una vez configurada la conexion a la base de datos, realizamos la migracion de datos y tablas a la base de datos mediante el comando:
```console
php artisan migrate
```

- Ya terminada la migración, podemos inicializar la API usando el siguiente comando:
```console
php artisan serve
```

### Vue JS

- Para inicializar la aplicacion web, necesitamos instalar las dependecias del proyecto, por lo que en un linea de comandos en la carpeta de **CrudVue** ejecutamos el siguiente comando:
```console
npm install
```

- Una vez se termine de instalar las dependencias, podemos inicializar nuestra aplicación web mediante el siguiente comando:
```console
npm run dev
```
Con esto, la aplicación estará funcionando de forma correcta.

## Desarrollador
- Aaron Steve Alfaro Zamora