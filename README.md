# Moodle-dockercompose


# Instalación del servicio Moodle y configuraración para la creacion de usuarios y cursos 

- instalacion y corrida con la herramienta docker - compose 


1- primer paso clonar el repositorio en nuestra maquina donde esta corriendo docker 

comandos:

$ git clone https://github.com/PabloLandaverde/Moodle-dockercompose.git
 
 se nos va a crear el directorio Moodle-dockercompose entramos a el con el siguiente comando:
 
 $ cd Moodle-dockercompose
 

2- segundo paso es correr el docker-compose yml con el siguiente comando:
 
 $ docker compose up
 
 
 3- al correr el docker compose nos arroja unos errores por lo tanto tenemos que detener los contenedores y se hace una configuracion con el superusuario (sudo) con los siguientes comandos:
 
$ sudo chgrp docker mariadb_data/

se utiliza para cambiar el grupo propietario de un directorio llamado "mariadb_data" al grupo "docker".

$ sudo chown 1001 mariadb_data/

se utiliza para cambiar el propietario de un directorio llamado "mariadb_data" al usuario con el identificador numérico 1001.
 
 
 4- una vez hecha las anteriores configuraciones con el superusario se ejecuta de nuevo el comando: 
 
 $ docker compose up
 

5- verificar que los contenedores se encuentren corriendo con el siguiente comando :
 
 $ docker ps
 

6- una vez que los contenedores esten corriendo en sus respectivos puertos, entramos a nuestro navegador e ingresamos localhost:90, oara acceder al servicio de moodle 


7- iniciar sesión con usuario y contraseña por defecto del servicio de moodle
  
  $ usuario :  user
  
  $ contraseña: bitnami
  

8 - una vez dentro configurar tu administrador a la persona designada 

#perfil

#editar perfil

llenar los datos que solicita 

- usuario
- contraseña
- correo electronico 

y guardar 


9- crear usuario

#  administrar usuario/ usuarios/ agregar usuarios


10- listar usuarios creados

administrar usuario/ usuarios/ listar usuarios
 
 
 
   
 







