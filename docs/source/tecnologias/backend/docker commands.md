#   COMANDOS PARA DOCKER

### Ejecutar bash de contenedor docker

>   docker run -it <image_name> /bin/bash

> or

>   docker exec -it <image_number> bash

Ejemplo

>   docker run -it mysql:5.5.48 /
bin/bash

NOTA: El nombre de la imagen se puede obtener con el comando docker ps -a


docker run 
-p 3305:3306
--name mysql-svv-puebla 
-v /docker/volume/mysql_puebla:/var/lib/mysql 
--network springcloud
-e MYSQL_ROOT_PASSWORD=cmsserverv6 
MYSQL_DATABASE=quartz_demo   
mysqld --lower_case_table_names=1
-d mysql:5.5.48





