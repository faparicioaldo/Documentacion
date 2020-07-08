#   Notas del aprendizaje de NPM y NPX.

##  NPM Gestor de paquetes incluido en la instalacion de NODE JS y NPX para ejecutar paquetes incluso sin descargarlos.

##  Instalacion

La istalacion del node js ya incluye NPM y NPX

>   https://nodejs.org/en/

1.  NPM: Gestor de paquetes de node.
2.  NPX: Ejecutor de paquetes sin descargar, Viene instalado con NPM 5.2+
    >   https://www.freecodecamp.org/news/npm-vs-npx-whats-the-difference/

Si la instalacion no funciona intentar:
1.  Abrir una consola nueva.
2.  Reinicial la maquina. 

##  Ruta de instalacion de paquetes NPM en windows
>   %AppData%/Roaming/npm

##  Comprobar instalacion
Ejecutar los comandos:
*   npm -v
*   npx -v

##  Desinstalar un paquete
Ejecutar comando:
    >   npm uninstall -g create-react-app

##  INSTALAR LA ULTIMA VERSION DE NPM
> npm install -g npm@latest

##  BORRAR CACHE NPM: SE HACE EN CASO DE ALGUN PROBLEMA AL DESCARGAR PAQUETES
> npm cache clean --force

##  utilizar paquete create-react-app sin descargarlo con NPX
> npx create-react-app myfirstapp
