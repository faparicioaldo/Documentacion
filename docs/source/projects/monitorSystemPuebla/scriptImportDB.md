#   EXPORTAR E IMPORTAR BASE DE DATOS DEL SERVIDOR

##  IMPORTAR BASE DE DATOS
"C:\Program Files (x86)\CMSServerV6\mysql\bin\mysql" -u root -pcmsserverv6 < C:\Users\Administrator\Desktop\Dump20200126.sql

##  EXPORTAR BASE DE DATOS - estructura
"C:\Program Files (x86)\CMSServerV6\mysql\bin\mysqldump" -u root -pcmsserverv6 quartz_demo > C:\Users\Administrator\Desktop\Dump08062020.sql

##  EXPORTAR BASE DE DATOS - datos
"C:\Program Files (x86)\CMSServerV6\mysql\bin\mysqldump" -u root -pcmsserverv6 --no-create-info quartz_demo >  C:\Users\Administrator\Desktop\quartz_demo_data.sql


##  EJECUTAR APLICACION JAVA
"C:\Program Files (x86)\CMSServerV6\tomcat\jdk1.8.0_162\bin\java" -jar c:\Users\Administrator\Desktop\SistemaMonitoreo-1.0.war


##  CONEXION A BASE DE DATOS
"C:\Program Files (x86)\CMSServerV6\mysql\bin\mysql" -h localhost -u root -pcmsserverv6


