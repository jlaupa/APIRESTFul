## TP Alquilando - API RESTful.

El objetivo de este TP es desarrollar una sencilla API RESTful que permita crear, obtener, actualizar y eliminar registros de una tabla MySQL. La API debe poder consumir y enviar la información en formato JSON.

<br>

Debe contener una tabla con los siguientes campos:
-	id
-	nombre
-	apellido
-	email
-	usuario

<br>

Endpoints necesarios:
-	POST /users (Crea un usuario)
-	GET /users (Obtiene la lista completa de usuarios)
-	GET /users/{user_id} (Obtiene el usuario de id {user_id})
-	PUT /users/{user_id} (Actualiza el usuario de id {user_id})
-	DELETE /users/{user_id} (Elimina el usuario de id {user_id})

## Instalacion del proyecto

Se uso el framework laravel([documentation](https://laravel.com/docs)) con tecnologias como InfyOm ([documentation](http://labs.infyom.com/laravelgenerator/docs/5.7/introduction) ).
<small>Aqui dejo un [link](https://www.powtoon.com/online-presentation/cVOdUOilMHo/?mode=presentation) para ver de que se trata. </small>

##Iniciando instalación

Teniendo un servidor con los requerimientos de laravel 5.7.

corremos los siguientes comandos en la consola:
- git clone https://github.com/miamius/APIRESTFul.git
- cd APIRESTFul
- composer install
- sudo chmod -R 777 storage

creamos la base de datos con nombre: alquilando2
y configuramos la url virtual en apache2 con la siguiente url : apirestful.test
continuamos: 
-php artisan migrate

y listo, ya tendriamos que poder la API
ejecutando la url : http://apirestful.test/api/docs
![Alt text](rpublic/images/leer_Doc_Api.PNG?raw=true "Api Doc")



