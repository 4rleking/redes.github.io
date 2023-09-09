---
layout: single
title: Modelo OSI
excerpt: ""
date: 2023-09-01
classes: wide
header:
  teaser: /assets/images/
  teaser_home_page: true
categories:
  - 
tags:
  - Modelo OSI
---

![](/assets/images/)

El *modelo OSI (Open System Interconnection)* organiza conceptualmente a las familias de protocolos de red en capas de red específicas. Este sistema de *interconexión abierto* tiene por objetivo  establecer un contexto en el cuál basar las arquitecturas de comunicación entre diferentes sistemas.

A continuación listamos algunos de los protocolos de red más conocidos, según las capas del *modelo OSI*:

## Protocolos de capa 1 (Capa Física)

* USB (Universal Serial Bus)
* Ethernet (Ethernet Physical Layer)
* DSL (Digital Subscriber Line)
* Etherloop (Combinación de Ethernet y DSL)
* Infrared (Infrared Radiation)
* Frame Relay
* SDH (Jerarquía Digital Sincrona)
* SONET (Red Optica Sincronizada)

## Protocolos de capa 2 (Enlace de Datos)

* DCAP (Protocolo de acceso del cliente de la conmutación de la transmisión de datos)
* FDDI (Interfaz de distribución de datos en fibra)
* HDLC (Control de enlace de datos de alto nivel)
* LAPD (Protocolo de acceso de enlace para los canales)
* PPP (Protocolo punto a punto)
* STP (Spanning Tree Protocol) [Protocolo del árbol esparcido]
* VTP VLAN (Trunking Virtual Protocol para LAN virtual)
* MPLS (Conmutación multiprotocolo de la etiqueta)

## Protocolos de capa 3 (Red)

* ARP (Protocolo de resolución de direcciones)
* BGP (Protocolo de frontera de entrada)
* ICMP (Protocolo de mensaje de control de Internet)
* IPv4 (Protocolo de Internet versión 4)
* IPv6 (Protocolo de Internet versión 6)
* IPX (Red interna del intercambio de paquetes)
* OSPF (Abrir la trayectoria más corta primero)
* RARP (Protocolo de resolución de direcciones inverso)

## Protocolos de capa 4 (Transporte)

* IL (Convertido originalmente como capa de transporte para 9P)
* SPX (Intercambio ordenado de paquetes)
* SCTP (Protocolo de la transmisión del control de la corriente)
* TCP (Protocolo del control de la transmisión)
* UDP (Protocolo de datagramas de usuario)
* iSCSI (Interfaz de sistema de computadora pequeña de internet iSCI)
* DCCP (Protocolo de control de congestión de datagramas)

## Protocolos de capa 5 (Sesión)

* NFS (Red de sistema de archivos)
* SMB (Bloque del mensaje del servidor)
* RPC (Llamada a procedimiento remoto)
* SDP (Protocolo directo de sockets)
* SMPP (Mensaje corto punto a punto)

## Protocolos de capa 6 (Presentación)

* TLS (Seguridad de a capa de transporte)
* SSL (Capa de conexión segura)
* XDR (External data representation)
* MIME (Multipurpase Internet Mail Extensions)

## Protocolos de capa 7 (Apliación)

* DHCP (Protocolo de configuración dinamica de host)
* DNS (Domain Name System)
* HTTP (Protocolo de transferencia de Hipertexto)
* HTTPS (Protocolo de transferencia de Hipertexto seguro)
* POP3 (Protocolo de oficina de correo)
* SMTP (Protocolo de transferencia simple de correo)
* Telnet (Protocolo de telecomunicaciones de red)

# TCP/IP y Modelo OSI

*TCP/IP* es una colección de protocolos estándar de la industria, diseñado para intercomunicar grandes redes *(WANs = Wide Area Networks)*. Las siglas TCP/IP provienen de *Transmission Control Protocol / Internet Protocol*.

Se creó en los 60's, cuando en los Estados Unidos se estaba desarrollando una forma de comunicación entre los puntos vitales de ese país. Pero no debía existir, ninguna "autoridad central", ya que sería el primer blanco de ataque, por lo tanto, esta red se decentralizó, así, toda máquina conectada a esta red tenía el mismo status y capacidad de controlar y recibir información.

Entonces, se decidió que los mensajes deberían dividirse en pequeñas porciones de información o paquetes, los cuales contendrían la dirección de destino, pero sin especifcar una ruta para su arribo; por el contrario, cada paquete buscaría la manera de legar al destinatario por las rutas disponibles y el destinatario reensamblaría los paquetes individuales para construir el mensaje original. Las rutas que siguen los paquetes no es de importancia, lo importante es la llegada a su destino.

En 1968, Inglaterra experimentaba con los mismos conceptos en el laboratorio Nacional de Física de la Gran Bretaña, estableciendose la primer red experimental británica. Por este motivo, el Pnetágono de E.E.U.U. comenzó a financiar un proyecto a través del Defense Advanced Research Projects Agency, DARPA.

Así, en 1969 DARPA establece la prime red universitaria en la Universidad de California (UCLA), surgiendo, tiempo después, nuevas redes adicionales, estableciendose ARPANET (Advanced Research Projects Agency Network).

En resultado de la aparición de esta nueva red, se fijaron protocolos afines que le permitieran la comunicación entre sistemas informáticos que contaban con diferentes tecnologías tanto en sistemas, como de comunicación. Por otra parte, se crearon diferentes alternativas de enlaces (links) de comunicaciones, pudiendo referirse a sistemas satelitales y de radio.

DARPA, fundó la compañía llamada *Bolt Beranck and Newman Inc.* que desarrolló la implementación de TCP/IP en BSD Unix. Este desarrollo ocurre al mismo tiempo que en muchos lugares se encontraban en proceso de adopción y desarrollo de tecnología de redes de áreas locales. Para enero de 1983, se encontraban en red todas las computadoras de ARPANET, utilizando los nuevos protocolos TCP/IP.

TCP/IP no es un simple protocolo, sino que consiste en una serie de protocolos, cada uno proveendo un servicio especifico, como http, ftp, e-mail, telnet, etc.

## Descripción del modelo OSI

Las redes de comunicaciones, están basadas en capas las cuales permiten la comunicación de los datos en una red. Para comprender la forma en que los protocolos trabajan, se han creados modelos de referencias. Los modelos más importantes son el *modelo OSI* y *TCP*.

El modelo OSI, se basa en la propuesta que desarrollo la Organización Internacional de Normas (ISO), siendo la primera estandarización de los protocolos (norma ISO 7494) que se usan en las diversas capas. Se llama a este, modelo de referencia OSI, por su significado (Open Systems Interconnection) Interconexión de sistemas abiertos.

El modelo OSI consta de 7 capas numeradas, donde cada una de ellas cumple una función especifica; las 7 capas del modelo OSI se ilustran a continuación.

## Capa 1 (Física)

La misión principal de esta capa es transmitir bits por un canal de comunicación, de manera que cuanto lo envíe el emisor, estas lleguen sin alteración al receptor.

La capa física proporciona sus servicos a la capa de enlace de datos, definiendo las especificaciones eléctricas, mecanicas, de procedimiento y funcionalidades para activar, mantener y desactivar el enlace físico entre sistemas finales, relacionando la agrupación de circuitos físicos a través de los cuales los bits son transmitidos.

Sus principales funciones las podemos resumir en:

* Definir las caracteristicas funcionales de la interfaz (componentes y conectores mecánicos) y eléctricos (niveles de tensión) que se van a usar en la transmisión de los datos por los medios físicos.
* Definir las caracteristicas funcionales de la interaz (establecimiento, mantenimiento y la liberación del enlace físico).
* Transmitir el flujo de bits a través del medio.
* Manejar voltajes y pulsos eléctricos.
* Especificar cables conectores y componentes de interfaz con el medio de transmisión, polos en un enchufe, etc.
* Garantizar la conexión (aunque no la fiabilidad de esta).

Esta capa solamente conoce bits indiviuduales.
En esta capa, los medios de transmisión que se encuentran son:

* Fisico
  * Par trenzado (twisted pair)
  * Cable coaxial
  * Fibra optica
* Inalambrico
  * Radio
  * Microondas
  * Infrarojo
  * Ondas de luz

## Capa 2 (Enlace de datos)

Proporciona sus servicios a la capa de red, suministrando un tránsito de datos confiable a través de un cable físico. Se ocupa del direccionamiento físico; la topología de red, el acceso a la misma, la notificación de errores, la formación y entrega ordenada de datos y control de flujo.

Su principal función es convertir el modo de transmisión en un medio de libre de errores de cualquier tipo, realizando para ello las siguientes funciones:

* Establecer los medios necesarios para una comunicación confiable y eficiente entre 2 máquinas en red.
* Agregar una secuencia especial de bits al principio y al final de los paquetes de datos, estructurando este flujo bajo un formato predefinido, denominado trama, que suele ser de unos cientos de bytes.
* Sincronizar el envío de los tramas, transfiriendolos de una forma confiable libre de errores. Para detectar y contratar errores se añaden bits de paridad, se usan CRC (Códigos Cíclicos Redundantes) y envía de acuses de recibo positivos y negativos, y para evitar tramas repetidos se usan números de secuencia en ellas.
* Controlar la congestión de la red.
* Regular la veocidad de trafico de datos.
* Controlar el flujo de tramas mediante protocolos que prohiben que el remitente envíe tramas sin la autorización explícita del receptor, sincronizando así su emisión y recepción.
* Encargarse el acceso de los datos al medio (soportes físicos de la red)

## Capa 3 (Red)

Proporciona sus servicios a la capa de transporte, siendo una capa compleja que proporciona conectividad y selección de la mejor ruta para la comunicación entre máquinas que pueden estar ubicadas en redes geográficamente distintas.

Es la responsable de las funciones de conmutación y enrutamiento de la información (direccionamiento lógico), proporcionando los procedimientos necesarios que conozca la topología de la red (forma en que están interconectados los nodos), con objeto de determinar la ruta más adecuada.

Las principales funciones son:

* Dividir los mensajes de la capa de transporte (segmentos) en unidades más complejas, denominadas paquetes, a los que asigna las direcciones lógicas de los hosts que se están comunicando.
* Conocer la topología de la red y manejar