---
layout: post
title: Barrio La Calleja
author: Andres Gomez
image: 
---

Primer barrio de Bogotá completamente mapeado por Maptime Bogotá.
Para este actividad usamos las siguientes técnicas:

 * Imágenes con drone.
 * Imágenes a nivel de calle.
 * Trazas GPS.
 * Herramientas de calidad de datos.
 
Para las imágenes de drone, tomamos fotos a una altura de 120 metros, y se recorrió el barrio con control manual.
Esta no es la mejor manera, ya que la perpectiva de los edificios no queda bien capturada, y algunos lugares no se alcanzaron a captar.
En el drone, se puso una toma de fotos cada 2 segundos para capturar la varias fotos; pero igualmente, por el vuelo manual, la velocidad no era constante.
 
Una vez se descargaron las fotos, se generó una imagen por medio de OpenDroneMap, con la opción de [WebODM](https://www.opendronemap.org/webodm/) que se instaló.
Como no eran muchas imágenes, la instalación fue suficiente, como también la máquina no requirió grandes capacidades de cómputo y terminó en pocos minutos (hubo un problema usandolo bajo Docker para Mac, por lo que se terminó usando directo bajo Linux Ubuntu.)
El resultado fue que generó un archivo TIF de casi 46 MB.

Con la imagen TIF, para compartirla con la comunidad se publicó en OpenAerialMap.
La imagen aerea de La Calle es [https://map.openaerialmap.org/#/-74.04922485351562,4.711955721595933,15/square/03223211212103131/604c3ffe5553510005076089?_k=fifm54](https://map.openaerialmap.org/#/-74.04922485351562,4.711955721595933,15/square/03223211212103131/604c3ffe5553510005076089?_k=fifm54)
Habiéndola publicado en este portal, el mapeo es más fácil, ya que solo debemos referenciar la imagen como un Imagery en TMS adicional; y no cargarla directamente en JOSM ya que puede consumir mucha memoria.

Igualmente, se tomaron fotos a nivel de calle, montadas sobre un carro, con una actionCam apuntando al frente, otra apuntando atrás, y una 360 en la mitad.
Todas estas fotos fueron más de 10 mil, por lo que se subieron de manera bulk a Mapillary.
Aquí se pueden ver todas esas fotos: [https://www.mapillary.com/app/?focus=map&lat=4.712011402221506&lng=-74.05024101516284&z=14.819927381168846](https://www.mapillary.com/app/?focus=map&lat=4.712011402221506&lng=-74.05024101516284&z=14.819927381168846)

Durante el recorrido en el carro, se aprovechó y se capturó una traza GPX con el celular.
La traza quedó publicada aquí: [https://www.openstreetmap.org/user/AngocA/traces/3573909](https://www.openstreetmap.org/user/AngocA/traces/3573909)

Con todos estos datos en terreno, se comenzó a mapear con JOSM (Se hizo la transición a OpenWebStart) y se fueron subiendo las contrucciones, vías y demás cosas que se identificaban.
Al principio, como íbamos a manejar un imagery nuevo, teníamos que estar seguros que estaba bien alíneado.
Como todo en el mundo de OSM, las características o features que no se conocen bien, es bueno estudiarlos.
En este caso estudiamos los hidrantes, la señales de altura, lugares de venta de carros, parques de juego (play ground).
Igualmente, para este mapeo, usando la opción de edificio (construcción) y después se unían varios con Shift + j para darle la forma definitiva.

Finalmente, con todos estos 

# Lexiones aprendidas

* Hacer las tomas desde drone cuando está un poco nublado es lo mejor, ya que no se proyectan sombras.

* En el carro, en vez de tener una cámara apuntando hacia atrás, se puede apuntar hacia la derecha para capturar las fachadas.
* Es bueno hacer las cargas de fotos a Mapillary de noche, para evitar consumir el ancho de banda durante el día. Esto, por estar en tiempos de pandemia y teletrabajo, beneficia a la comunidad.
* Los commits deben venir un un HashTag para poder asociar todos los commits de esta actividad.
* Leer el wiki de OSM cuando hay un feature que no se le conocen los detalles.
