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

## Instalación del proyecto

Se usó el framework laravel([documentation](https://laravel.com/docs)) con tecnologías como InfyOm ([documentation](http://labs.infyom.com/laravelgenerator/docs/5.7/introduction) ).
<small>Aquí dejo un [link](https://www.powtoon.com/online-presentation/cVOdUOilMHo/?mode=presentation) para ver de qué se trata. </small>

##Iniciando instalación

Teniendo un servidor con los requerimientos de laravel 5.7.

corremos los siguientes comandos en la consola:
- git clone https://github.com/miamius/APIRESTFul.git
- cd APIRESTFul
- composer install
- sudo chmod -R 777 storage

creamos la base de datos con nombre: alquilando2
y configuramos la url virtual en apache2 con la siguiente url : apirestful.test (*)
continuamos: 
-php artisan migrate

y listo, ya tendriamos que poder ver la API corriendo.
ejecutando la url : http://apirestful.test/api/docs
![Alt text](public/images/leer_Doc_Api.PNG?raw=true "Api Doc")

============================================================================
En el caso de que uses windows y no tengas linux a disposición con todos los requerimientos de laravel.Puedes probar el siguiente método rápido!
Descárgate [laragon](https://sourceforge.net/projects/laragon/):
-Inicializalo
-Abre el terminal de laragon
-posicionate en ...\laragon\www
-Realiza el git clone https://github.com/miamius/APIRESTFul.git
-Detén el servicio(boton "detener") y vuelvelo a iniciar
-Abre el terminal de nuevo, dirigete a la carpeta apirestful
-corre: composer install, chmod -R 777 storage
-crea un base de datos con el nombre :alquilando2
-Ahora en el terminal corre:php migrate
-Fin.

Imagenes de muestra que este proyecto funciona: directorio "public/images"

![Alt text](public/images/fin.PNG?raw=true "Fin")
Éxitos!
Cualquier consulta mi email es jairo.laupa@gmail.com

<small>Fecha28/10/2018__Hora inicio: 17horas , Hora de finalización:19:18</small>
