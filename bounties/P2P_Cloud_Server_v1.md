![alt text](https://github.com/bitDubai/media-kit/blob/master/MediaKit/Fermat%20Branding/Fermat%20Logotype/Fermat_Logo_3D.png "Fermat Logo")

# Herramientas de Supervision y Control para el Servidor (Cloud Server)

## Introduccion

La interconexion entre sistemas, y aplicaciones distribuidas corriendo en diferentes dispositivos es una de las necesidades fundamentales en era de la globalización e internet, esta necesidad de compartir y buscar información es solventada atraves de las redes. Fermat no escapa de esta necesidad y uno de sus primeras metas es contar con una Red Peer to Peer (The Fermat Network) para el intercambio de toda su metadata, e información relevante para su funcionamiento.

Las redes P2P permiten el intercambio directo de información, en cualquier formato, entre los dispositivos interconectados, una serie de nodos que se comportan como iguales entre sí, los cuales proveen y aportan el ancho de banda y computo distribuido para los recursos que hacen funcionar la red. Las redes P2P tienen muchas ventajas grandes e importantes, pero una de sus mayores problemas es su implemetación debido a la complegidad que involucra como por ejemplo: la mayor parte de los nodos de Internet no disponen de una dirección IP fija o siquiera accesible para otros nodos de Internet,  los nodos que se conectan a través de redes locales como Wifi o Ethernet, de aquellos que tienen algún tipo de cortafuegos y NAT. 

En Fermat mientras que se desarrollamos o implemntamos nuestra red Peer to peer (The Fermat Network), hemos desarrollado un preview de la misma basada en una arquitectura Cliente-Servidor (Cloud Client y Cloud Server) la cual tiene como fin solventar temporalmente la necesidad de interconexion y comunicaciones del sistema. La arquitectura cliente-servidor es un modelo de aplicación distribuida en el que las tareas se reparten entre los proveedores de recursos o servicios, llamados servidores, y los demandantes, llamados clientes. Un cliente realiza peticiones a otro programa, el servidor, quien le da respuesta.

## Alcance

## Propósito general

En el paradigma de Cliente - Servidor clásico no tiene la robustez de una red P2P. Cuando un servidor está caído, las peticiones de los clientes no pueden ser satisfechas. En la mayor parte de redes P2P, los recursos están generalmente distribuidos en varios nodos de la red. Aunque algunos salgan o abandonen la descarga; otros pueden todavía acabar de descargar consiguiendo datos del resto de los nodos en la red. Debido a esto es importante la supervision temprana de los mismos.

### Desarrollo Actual

En el presente se cuenta con dos componenetes (plug-ins):

El Servidor (Cloud Server) es un programa idependiente que puede ser ejecutado en una computadora, y el cual tiene la resposabilidad de interactuar entre todos los clientes para transmitir los datos deseados entre ellos.

El Cliente (Cloud Client) este plugin es el encargado de la interaccion con el servidor y contruir e interpretar los paquetes de datos necesarios para ser enviados y recibidos desde el servidor (Cloud Server)

### Alcance del Bounty

#### Tabla de elementos u objetivos a cumplir



---
| N° | Objetivo | Descripción | Porcentaje |
|:--:|:--------:|:-----------:|:-------------:|
| 1 |Monitoreo	| Implementar una herramienta de monitoreo, en la cual se pueda observar el estatus del servidor, en el cual se observer datos básicos como: Memoria utilizada, Carga del Cpu, Tiempo de ejecución entre otras.|  |
| 2 | Alertas y Notificaciones | Implementar mecanismo de notificación y alerta  cuando el servidor no este disponible, o presente fallas u quede poco espacio en disco |  |
|3| Guía de Instalación | Elaborar una guía detallada de instalación y configuración del servidor en cualquier computador | |
|4| Pruebas de Estrés |	Implementar pruebas de estrés para verificar el comportamiento y rendimiento del servidor en cuanto a concurrencia y sobre carga de peticiones, y elaborar un informe final con los resultados de la mismas  |  |
---

## Línea de tiempo

Sobre la base de la carga de trabajo y los recursos actuales disponibles, la fecha de entrega de esta recompensa (bounty) será **15 de Marzo**.

## Evaluación

Para ser considerado éxitozo esta recompensa (bounty) debe superar los siguiente:

* Todos los elementos anteriormente expuesto debe ser realizados.

* La evaluación que se realizará será en base a lo aportado, por cada uno de los desarrolladores. Se realizará un calculo matematico para determinar cuanto a sido el aporte de la persona para completar el bounty en base a la cantidad de elementos realizados con exito.


*[Resultados de la evaluación para ser completado después de la evaluación]*

## Distribución

*[Distribution to be completed after evaluation]*

| N° | Objetivo  | Desarrollador | Completado |
|:--:|:---------:|:-------------:| :-------------:|
| 1  | Monitoreo | Roberto Requena ||
| 2  | Alertas y Notificaciones | Roberto Requena | |
| 3  | Guía de Instalación | Roberto Requena | |
| 4  | Pruebas de Estrés | Hendry Rodriguez | |
