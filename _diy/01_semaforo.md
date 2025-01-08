---
title: "Crear un semaforo con una placa Arduino"
image: 
  thumbnail: docs/images/semaforo01.png
categories:
  - DIY
tags:
  - Scalextric
  - Arduino
---

# Crear un semáforo con una placa Arduino

Para las carreras realizadas en el club era necesario contar las vueltas y los tiempos. En los primeros campeonatos esto se hacía de forma manual con un simple cronometro, pero esto resultaba ineficiente y poco preciso, dando muchos problemas.	
Actualmente, el club cuenta con un semáforo digital de la marca Carrera. Este semáforo permite contar vueltas y tiempos además de dar la salida.

Pero antes de que el club pudiera comprarse un semáforo, se las tuvo que ingeniar para crear un semáforo casero que tuviera las mismas funcionalidades que uno comercial. Por ello, CHAMO DESIGN inventó un semáforo fundamentado en Arduino y con sensores de infrarrojo para la detección de movimiento.

Los materiales utilizados para este semáforo fueron:
-	Arduino UNO.
-	Sensores SHARP infrarrojos.
-	Pantalla LCD.
-	Marco de madera.
-	Leds.
-	Resistencias varias.
-	Batería 9V (opcional).
-	Potenciómetro (opcional).
-	Controlador infrarrojo (opcional).
-	Zumbador (opcional).
-	PCB (opcional).

Los materiales marcados como opcional no serían necesarios para el proyecto pudiendo cambiarlos por otros o simplemente no usarlos.

Los sensores basados en luz infrarrojos permiten medir distancias sin muchas interferencias entre ellos. El funcionamiento de estos sensores se basa en medir la distancia constantemente. El sistema cuanta esta distancia como un 0 y cuando la distancia cambia, pasando un coche por el sensor, es un 1. Este funcionamiento de lógica digital y flancos de subida es muy útil para el caso del semáforo. Con la utilización de la detección de flancos de subida, se evitan que el semáforo cuente más de una vuelta.
El semáforo cuenta con una pantalla LCD para visualizar los tiempos y las vueltas realizadas de forma clara. Se podría visualizar usando otros métodos como una pantalla TFT pero con la pantalla LCD se cumplen las funcionalidades básicas.
Los Leds servirán para marcar la salida de los coches o marcar otros eventos como la realización de una vuelta o la finalización de la carrera. Serán necesarias añadir unas resistencias de 330 Ω para que no se quemen los leds.
Para alimentar el semáforo se puede usar una batería de 9V conectada a la placa Arduino. También se puede usar una toma de corriente que transforme los 220V en alterna de la red a los 9-12V en continua que necesita el Arduino.
El potenciómetro está incluido para calibrar la distancia que miden los sensores. El controlador de infrarrojos se añadió para controlar el sistema del semáforo de forma remota. El zumbador también sirve para señalizar las vueltas.
Por último, se diseñó una PCB para evitar el exceso de cables y la simplicidad en el montaje. Se puede sustituir por una protoboard y pines, pero tendría una apariencia más descuidada.
Todo el código utilizado en este semáforo se puede encontrar en el repositorio de CHAMO DESIGN. En un principio se programó el semáforo para que se establecieran cada piloto y estableciera los enfrentamientos entre estos. Esto sería complicar demasiado el diseño, por eso, es mejor reducir las características del semáforo a las más básicas.
Durante las pruebas del semáforo, este media con bastante exactitud las vueltas y tiempos de los coches. La interfaz que se utilizo fue demasiado complicada pudiendo reducirse en diseño, eliminando elementos innecesarios como el controlador o el zumbador y reduciendo líneas de código considerablemente.

![](../docs/images/semaforo01.png)


![](../docs/images/semaforo02.png)


![](../docs/images/semaforo03.png)
