# API RESTful con Node.js

Proyecto de demostración para clases de desarrollo de APIs utilizando Node.js,
con implementación del CMS (Strapi) de codigo abierto basado en Node.js.

## Tabla de contenido

- [API RESTful con Node.js](#api-restful-con-nodejs)
  - [Tabla de contenido](#tabla-de-contenido)
  - [Requisitos de instalación](#requisitos-de-instalación)
  - [Instrucciones para la instalación](#instrucciones-para-la-instalación)
  - [Documentación detallada](#documentación-detallada)
  - [Enlaces externos](#enlaces-externos)

## Requisitos de instalación

Asegúrate de tener instalado Node.js, Xampp y Postman.

- [Xampp](https://www.apachefriends.org/download.html)
- [Postman](https://www.postman.com/)
- [Node.js](https://nodejs.org/en)

## Instrucciones para la instalación

1. Clonar el repositorio en la máquina local:
   
   ```sh
   git clone https://github.com/KatoGC/T4-01-Proyecto.git
   ```

2. Navegar al directorio del proyecto:
   
   ```sh
   cd T4-01-Proyecto.git
   ```

3. Ejecutar el siguiente comando para intalar strapi:

    ```sh
    npm install strapi@latest
    ```
    
4. Ejecutar el siguiente comando para hacer la construccion:

    ```sh
    npm run build
    ```
    
5. Ejecutar el siguiente comando para iniciar los contenedores:

    ```sh
    npm run develop
    ```
    
    > **IMPORTANTE**
    >
    > 
    >Debe tener inicalizado los servicios de Apache y MySQL en Xampp

6. La API estará disponible en `http://localhost:1337`.

7. El panel de adminstración estará disponible en `http://localhost:1337/admin`

## Documentación detallada

Para obtener información detallada sobre los endpoints y cómo utilizar la API,
consulta la [documentación detallada](./src/api/README.md).

## Enlaces externos

- [Xampp](https://www.apachefriends.org/download.html)
- [Postman](https://www.postman.com/)
- [Node.js](https://nodejs.org/en)
