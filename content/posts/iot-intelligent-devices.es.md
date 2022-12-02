---
title: IOT - Dispositivos Inteligentes
date: 2022-12-02
tags:
    - IOT
    - leyes
    - futuro
    - tecnología
cover: images/iot-intelligent-devices.jpg
---

Hace poco descubrí que mi robot aspirador dejó de funcionar durante más de tres días.

No podía configurar el programa de aspirado, es decir, no podía modificar el plan de limpieza para definir las habitaciones a limpiar ni modificar la potencia de succión que la aplicación te permite configurar **y no puedes hacerlo de ninguna otra forma**.

<!--more-->

#### ¿Entonces?

En realidad, puedes encender el robot con el botón que trae el propio aparato y este realizará el último recorrido con el que fue configurado. Con suerte será la casa completa a una potencia de succión suficiente.

Pasados unos días, la aplicación volvió a funcionar... pero esto me hizo reflexionar. Dependemos de servicios de terceros cuando compramos ciertos productos, como robots aspirador, enchufes inteligentes, cámaras de vigilancia, etc.

Ante esta situación hay *(principalmente)* dos grupos de personas:

- **Gente común** que no tiene por qué conocer estos detalles y compra este tipo de dispositivos porque les gusta o los necesitan.
    Creen que pueden ser una buena solución para ellos, pero que ante este tipo de situaciones, lo único que pueden hacer es llamar al comercio donde lo compró o llamar al fabricante para gestionar la garantía.
- **Informáticos** o a los que nos gusta resolver problemas tecnológicos y entendemos cómo funciona este tipo de dispositivos, es decir, sabemos que estos se conectan a un servidor remoto para enviar/recibir datos *(cosa que no nos suele gustar)* y que necesitamos para interactuar con ellos desde dentro y fuera de casa a través de una aplicación.

#### Cámaras de vigilancia

Estos aplica también a cámaras de vigilancia. El uso común de una cámara de vigilancia es ser capaz de ver lo que pasa en la vivienda en tiempo real desde cualquier lugar. Además, ante cualquier evento/movimiento recibir notificaciones de seguridad. Para esto confiamos, de forma implícita, en servicios externos.

¿Son conscientes los usuarios de como funciona esto? Si supieran que las imágenes pasan por un servidor de una empresa *(que puede ser o no la fabricante del producto)*, se analiza el contenido y se almacena en la nube, ¿Lo comprarían? ¿Lo usarían? ¿Lo instalarían en su casa?

El público general no tiene por qué conocer este detalle, para la mayoría solo se trata de una aplicación la cual configura la cámara de vigilancia y mágicamente puede ver lo que pasa en su casa desde cualquier parte del mundo.

Pero **la magia no existe**, en esto estamos todos de acuerdo.

#### Alternativas

Encontré un grupo de afectados *(en telegram)* y resulta que no era el único... El motivo fue que los servidores de esta marca se cayeron y estuvo fuera de servicio durante ese fin de semana por completo.
En este grupo de telegram descubrí que existía una forma por la cual montar un servidor compatible por cuenta propia. De esta forma, yo sería el único responsable de mantener el servicio funcionando para poder usar mi robot aspirador y poder configurarlo sin necesidad de depender de esa tercera empresa.

Tras varias horas de leer información y tras estudiar *(no es trivial)* cómo se podía acceder y re-configurar *(rootear)* el robot para que usara este nuevo método, finalmente lo hice funcionar.
Todo esto solo es viable si eres informático y te gustan este tipo de cosas.

#### Futuro

Para el público general preveo problemas legales con las garantías, es decir:
- ¿Qué pasa si tu robot aspirador deja de funcionar?
- ¿Qué pasa si te deja de dar cierta funcionalidad si un servidor de una empresa deja de funcionar?
- ¿Qué pasa si la empresa quiebra?
- o... cualquier otro motivo que haga que no puedas utilizar esa aplicación para configurar tu dispositivo...

*¿Existe algún tipo de ley que obligue tener que soportar y proveer servicios durante al menos la vida útil del dispositivo?*

Si no es así...

*¿Qué responsabilidad tiene la empresa de mantener el servidor o ese servicio más allá de un año o dos años desde la venta del producto?*

Es decir, podíamos llegar a un punto en el que tu dispositivo sea un pisapapeles. ¿Verdad? **Incluso estando en buen estado**.
Puede llegar el momento en que no puedas usar tu dispositivo para nada porque la empresa ha dejado de dar servicio y todo eso va directamente
al chatarrero.

Preveo las siguientes situaciones:

- Legislar para evitar estas situaciones. Tiene lagunas:
  - ¿Cómo se puede obligar a una empresa fuera de la unión europea a dar un servicio durante la vida útil de un dispositivo?
- Vuelta a los dispositivos no inteligentes.
  - El consumidor preferirá gastarse más dinero y que su dispositivo funcione independientemente de si la empresa quiebra y así poder disfrutar plenamente de su dispositivo.
- Empresas que se dediquen a dar servicio de mantenimiento de estos dispositivos
  - *No suele ser económicamente viable*
