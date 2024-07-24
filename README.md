# Apilados - Sistema de Gestión de Libros - Sebastian Ahern

## Descripción

**Apilados** es una aplicación multiplataforma diseñada para la gestión interna de libros en la librería Apilados. La aplicación permite a los empleados ingresar, modificar, eliminar, listar y buscar información de los libros disponibles. El backend de la aplicación está construido con Node.js y MongoDB, mientras que el frontend utiliza React. La aplicación se despliega en dispositivos Android utilizando Apache Cordova.

## Características

- **Ingreso de Libros:** Permite agregar nuevos libros al sistema.
- **Modificación de Libros:** Permite actualizar la información de los libros existentes.
- **Eliminación de Libros:** Permite eliminar libros del sistema.
- **Listado de Libros:** Muestra una lista de libros con detalles como nombre, autor, editorial y portada.
- **Búsqueda de Libros:** Permite buscar libros por nombre, autor o editorial.
- **Visualización Detallada:** Muestra información detallada de cada libro con enlaces para actualizar o eliminar.

## Tecnologías Utilizadas

### Backend
- Node.js
- Express
- MongoDB
- Mongoose
- Validator

### Frontend
- React
- React Router DOM
- Axios
- Simple React Validator

### Deployment
- Apache Cordova
- Android Studio
- Gradle

## Instalación y Ejecución

### Requisitos Previos

- Node.js y npm
- MongoDB
- Apache Cordova
- Android Studio

### Pasos para la Instalación

1. **Clonar el Repositorio:**
   ```sh
   git clone <URL_DEL_REPOSITORIO>
   cd apilados

2. **Configuracion del Backend:**

    ```sh
    cd server

 Navega al directorio del servidor:
sh
Copy code
cd server
Instala las dependencias:
sh
Copy code
npm install
Crea un archivo .env con la configuración de la base de datos:
env
Copy code
MONGO_URI=<TU_URI_DE_MONGODB>
PORT=5000
Inicia el servidor:
sh
Copy code
npm start
Configuración del Frontend:

Navega al directorio del cliente:
sh
Copy code
cd ../client
Instala las dependencias:
sh
Copy code
npm install
Inicia la aplicación de desarrollo:
sh
Copy code
npm start
Configuración de Apache Cordova:

Navega al directorio de Cordova:
sh
Copy code
cd ../cordova-app
Agrega la plataforma Android:
sh
Copy code
cordova platform add android
Copia los archivos de construcción de React al directorio www:
sh
Copy code
cp -r ../client/build/* www/
Construye y ejecuta la aplicación en un dispositivo Android:
sh
Copy code
cordova build android
cordova run android
Uso
Una vez que la aplicación esté en ejecución, podrás interactuar con ella a través de la interfaz gráfica proporcionada en el frontend. Utiliza el menú de navegación para acceder a las diferentes funcionalidades como agregar, modificar, eliminar, listar y buscar libros.