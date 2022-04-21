## Objectivo
- Este proyecto muestra Express + Swagger + Serverless + Lambda + Dynamondb + ClaudiaJS
- Express se utiliza como marco de back-end
- ClaudiaJS se utiliza para implementar el código Express en una arquitectura sin servidor en AWS API  Gateway con tecnología Lambda
- Swagger para documentación (duh) - más importante aún, cómo se realiza la documentación dentro del propio código para que siempre pueda estar actualizado
- Dynamondb como bd no Sql en la nube

## Instruciones
- Antes de todo ejecutar para un deploy hacer test unitarios probar si en local funciona el servidor y el metodo Get creado funciona.
- Para ejecutar el código: `npm run start`
- Para implementar por primera vez en AWS: `npm run claudia-init`
- Implementaciones posteriores en AWS: `npm run update-api`
- En consola ejecutar el comando serverless deploy --verbose, este comando subira al aws nuestra aplicacion creando IAM con rol de user, tambien, log del grupo o usuario que se creo al principio en aws con los permisos .

## Librerias Usadas
- `swagger-jsdoc`
- `swagger-ui-express`
- `claudia`
- `aws-serverless-express`
- `node-fetch`
-  

### Invocación

Después de una implementación exitosa, puede llamar a la aplicación creada a través de HTTP:

- Cree un metodo Get HTTP con la dependencia Fetch me trae de la API de prueba SWAPI un pequeño json.

### Base de datos AWS DynamoDB

Integración: la integración de esta base e datos no sql que nos proporciona aws lo podemos hacer de 2 formar ingresando al tableblero en aws y buscamos DynamoDB creariamos la bd con sus colecciones, pero en este proyecto estoy usando ( SERVERLESS ) serverless nos da la ayuda de crear nuestra bd en el archivo de configuración ( Serverless.yml ) creando asi  nombre db, coleccciones para asi poder subir ya todo listo al aws al ejecutar el comando ya antes mencionado (serverless deploy --verbose )  

