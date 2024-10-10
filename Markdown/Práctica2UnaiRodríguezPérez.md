# Configuración de un Servidor DHCP en Debian

## EJERCICIO 1: 

### 1. Instalación del Servidor DHCP
Para instalar el servidor DHCP en Debian, abre una terminal y ejecuta los siguientes comandos:
![1](/apt-get%20install%20isc-dhcp-server.PNG)
![2](/Captura.PNG)

Configuraciones necesarias para tener un rango de ips, el dns, nombre del dominio, la puerta de enlace y el tiempo mínimo y máximo de estancia.

![3](/Captura1.PNG)
![4](/rango%20de%20ips.PNG)
![5](/Host%20cliente1.PNG)
![6](/DNS%20debian.PNG)

## EJERCICIO 2:
Configuramos los cliente de DHCP:

Ponemos el Windows en DHCP para que el servidor de Debian asigne la ip al cliente de Windows.

![7](/DHCP%20windows.PNG)

Ponemos el Ubuntu en DHCP para que el servidor de Debian asigne la ip al cliente de Ubuntu.

![8](/DHCP%20ubuntu.PNG)

Vemos que ips nos han asignado por el servidor de Debian:

![9](/Ver%20que%20ips%20han%20sido%20asignadas.PNG)

Cliente de Windows:

![10](/Ipconfig%20all%20Windows.PNG)

Cliente de Ubuntu:

![11](/IP%20A%20ubuntu.PNG)

Verificación de los equipos:

Windows

![12](/Ping%20de%20windows%20a%20debian.PNG)
![13](/Ping%20google%20Windows.PNG)

Ubuntu

![14](/Ping%20de%20ubuntu%20a%20debian.PNG)
![15](/Conexion%20google%20Ubuntu.PNG)

## EJERCICIO 3:
Actividad del servidor capturada con el Journalctl.

En esta captura muestra los procesos ejecutados después de realizar un restart a la carpeta de interfaces.
Lo primero que hace es parar el servicio , seguido te muestra un mensaje de que el servicio a sido parado exitosamente, mas tarde en un color verde claro la maquina va a volver a encender ese proceso y ya los próximos mensajes son de que ese proceso ya está puesto en funcionamiento.

![16](/Journal.PNG)
