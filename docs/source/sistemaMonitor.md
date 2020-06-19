# Sistema de Monitoreo Puebla
## Funcionamiento del Sistema

### Introduccion
El proyecto sistema de monitoreo es un sistema intermediario entre el sistema ceiba2 y los sistemas de la secretaria de movilidad (SEMOVI) de la ciudad de puebla.

El sistema de monitoreo realiza dos acciones:
*   Envio de GPS en tiempo real de los vehiculos registrados.
*   Envio de alertas por boton de panico.

IMPORTANTE: El sistema de monitoreo requiere la captura de datos complementarios de cada vehiculo que se obtiene de CEIBA2, si esta condicion no se cumple el sistema no realizara las funciones descritas en el parrafo anterior.

### Envio de GPS en tiempo real de los vehiculos registrados.
Para el envio de GPS de cada vehiculo el sistema monitoreo realiza los pasos siguientes: 
*   Se obtiene datos necesarios de cada vehiculo del sistema CEIBA2 mediante un API que este ultimo expone en javascript y se guardan en una lista desordenada.
*   Se obtienen datos complementarios de cada vehiculo del sistema de monitoreo.
*   Se crea una cadena con un formato especifico que contienen los datos recebados en los dos pasos anteriores para cada vehiculo registrado.
*   Se realiza en el envio de datos de GPS para cada vehiculo hacia SEMOVI via TCP-IP.
*   Los pasos anteriores se repiten cada 2 segundos para enviar GPS de cada vehiculo de manera periodica y constante, esto se hace utilizando un sheduler en Java.

### Envio de alertas por boton de panico.


### Controller del model MVC en el proyecto:
*   AmbienteController
*   MostrarCadenasController
*   UserController
*   DatosVehiculoController (IMPORTANT)
*   MonitorAlarmasController (IMPORTANT)
*   MonitorFoliosAlarmasController (IMPORTANT)
*   VideoController (IMPORTANT)


