#   Proyecto Sistema de Monitoreo Puebla
##  Definicion de reglñas de negocio

### Introduccion
En el presente documento se describen las reglas de negocio implementadas para el funcionamiento del sistema de monitoreo para la ciudad de Puebla.

### Reglas de Negocio
1.  Mostrar listado de vehiculos registrados en ceiba2 (datosVehiculos).
2.  Registrar un nuevo vehiculo (agregarVehiculo):
    *   Aun que el vehiculo exista en ceiba2 el sistema no lo detecta se debera ingresar manualmente.
3.  Agregar una alerta (agregarDatosAlarma)
    *   Solo se agrega si no fue registrada previamente lo cual se valida con un id otorgado por ceiba2.

### Funcionalidades Principales Sistema
1.  Solicitar relacion de nuevos registros de alertas en ceiba2 (solo estatus 13 y 5).
2.  Validar alertas una a una si son nuevas o ya han sido procesadas.
3.  Validar si datos complemento ya han sido capturados en este sistema.
4.  Armar cadena con datos de ceiba2 y datos complemento, se incluye URL de 4 videos de camaras.
5.  Enviar cadena de alertas nuevas a semovi.
6.  Registrar respuesta de semovi en bitacora.
7.  Registrar alertas nuevas en tabla para control de enviadas.
8.  Informar al front via websocket de las nuevas alertas enviadas a semovi.
9.  **Crear vista** para mostrar alertas enviadas a semovi en orden descendente.
10. **Crear vista** para mostrar errores al enviar alertas de panico a semovi.
11. **Crear vista** para mostrar vehiculos registrados en ceiba2 y en monitor.
12. **Crear vista** para mostrar vehiculos registrados en ceiba2 y pero NO en monitor.
13. **Crear vista** para errores al enviar GPS.
14. **Crear vista** para mostrar 4 videos de vehiculo con posibilidad de elegir tambien indicar si no han sido capturado datos complementarios en monitor
