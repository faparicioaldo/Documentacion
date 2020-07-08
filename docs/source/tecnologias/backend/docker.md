#   Comandos docker

------------------------------------------------------------------------------------
------------------------------------------------------------------------------------
--COMANDOS DOCKER - CURSO SPRING CLOUD - UDEMY
--CURSO: https://www.udemy.com/course/microservicios-con-spring-boot-y-spring-cloud
------------------------------------------------------------------------------------
------------------------------------------------------------------------------------

------------------------------------------------------------------------------------
--MOVERSE A CARPETAS DE PROYECTOS
cd C:\FONACOT\Workspace_TUTORIALES\springboot-servicio-config-server\
cd ..\springboot-servicio-eureka-server\ 

------------------------------------------------------------------------------------
--CREAR RED CON DOCKER
docker network create springcloud 

------------------------------------------------------------------------------------
--COMPILAR DOCKERFILE PARA CREAR IMAGEN
docker build -t eureka-server:v1 . 

------------------------------------------------------------------------------------
--EJECUTAR CONTENEDOR INDICANDO PUERTOS, IMAGEN, RED, Y TAG O VERSION DE LA IMAGEN
docker run -ip 8888:8888 --name config-server --network springcloud config-server:v1 
docker run -ip 8761:8761 --name eureka-server --network springcloud eureka-server:v1 

docker images
docker image ls

------------------------------------------------------------------------------------
--DESACRGAR IMAGEN MYSQL 8 DE REPOSITORIO DOCKER HUB
docker pull mysql:8

------------------------------------------------------------------------------------
--CREAR CONTENEDOR CON BASE DE DATOS MYSQL 8, SE INDICA PUERTOS, RED, CONTRASEÑA DE ROOT Y VERSION DE LA IMAGEN

En el comando siguiente primero se indica el puerto local seguido del puerto del contenedor.

docker run -p 3307:3306 --name microservicios-mysql5.5.48 --network springcloud -e MYSQL_ROOT_PASSWORD=cmsserverv6 -e MYSQL_DATABASE=db_springboot_cloud -d mysql:5.5.48



docker run -p 3306:3306 mysql:5.6 -e MYSQL_ALLOW_EMPTY_PASSWORD=1 mysqld --lower_case_table_names=1
------------------------------------------------------------------------------------
--MOSTRAR LOG DE CONTENERDOR DE MYSQL 8
docker logs -f microservicios-mysql8


