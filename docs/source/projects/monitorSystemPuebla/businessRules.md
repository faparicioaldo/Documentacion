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
    