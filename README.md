# flow4-NodeRed-MQTT
Este repositorio contiene el flow 4 del curso de NodeRed, visto en en los contenidos de Internet de las cosas de Codigo IoT en edu.codigoiot.com

# Introducción
Este flow consiste en un tablero que presente la información de temperatura y humedad locales. Este flow recibe la información por MQTT con un broker local.
# Material Necesario
Para realizar este flow necesitas lo siguiente

   [Ubuntu 20.04](https://releases.ubuntu.com/20.04/) 
  
   [ NodeJS](https://nodejs.org/es/)
   
   [ NPM](https://www.npmjs.com/)
       
   [NodeRed](https://nodered.org/docs/getting-started/local)
        
   [  Nodos Dashboard](https://flows.nodered.org/node/node-red-dashboard)
   
   [  Mosquitto]([https://flows.nodered.org/node/node-red-dashboard](https://mosquitto.org/))
      
# Material de referencia
En los siguientes enlaces puedes encontrar cursos en la plataforma de edu.codigoiot.com que te permitirán realiar las configuraciones necesarias



   [Instalación de Virutal Box y Ubuntu 20.04](https://edu.codigoiot.com/course/view.php?id=812)
   
   [Instalación de NodeRed](https://edu.codigoiot.com/enrol/index.php?id=817)
   
   [Introducción a NodeRed](https://edu.codigoiot.com/enrol/index.php?id=278)
   
   [Introduccion a Mosquitto]([https://edu.codigoiot.com/enrol/index.php?id=278](https://edu.codigoiot.com/course/view.php?id=851))


# Instrucciones
Requisitos previos
Para que este flow funcione, debes cumplir con los siguientes requisitos previos

Instalación de NodeJS. Se recomienda tener instalado NodeJS en alguna versión LTS. Al momento de creación de este documento, se usó la versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM


Instalación de NodeRed. La instalación se realiza por NPM. Al momento de la creación de este contenido, se usó la versión 3.0.2


Instalar los nodos node-red-dashboard. Para ello, dirigete a la opcion "Manage Palet" de NodeRed y en la pestaña Install busca node-red-dashboard. Finalmente haz clic en instalar.


Instalación de Broker local Mosquitto MQTT.


Instrucciones de preparación del entorno
Para ejecutar este flow, es necesario lo siguiente

Arrancar NodeRed con el comando node-red

Importar el flow del repositorio

Hacer clic en el boton Deploy

Instrucciones de operación

Para observar el resutlado de este flow, abre un navegador y dirígete a localhost:1880/ui

Enviar por MQTT un mensaje que contenga un JSON con las variables ID, temp y hum
    
Notas
Este Flow se suscribe al tema codigoIoT/Mor/mqtt/flow4

El mensaje mqtt usado para probar este flow es mosquitto_pub -h localhost -t codigoIoT/Mor/mqtt/flow4 -m '{"ID":"Ian Arcos","temp":21,"hum":51}'

Para que la gráfica historica muestre información, deben enviarse al menos 2 puntos

# Resultados
A continuación puedes ver los nodos del flow.
![Captura de pantalla del flow 3](https://user-images.githubusercontent.com/111370977/186721102-13084e27-2c88-47a7-8bd1-ff883d8942c3.png)

A continuación puede ver el tablero resultante.

![Captura de pantalla del flow 3-2](https://user-images.githubusercontent.com/111370977/186721118-68b46f35-3a79-4c8b-822d-315544407e0c.png)



# Evidencias







https://user-images.githubusercontent.com/111370977/186721904-98e87cfc-53ed-4a11-9480-d6bc4d8f8ff4.mp4





# Creditos
Desarrollado por Ian Arcos

https://github.com/ArcosIan
