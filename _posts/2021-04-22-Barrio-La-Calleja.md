---
layout: post
title: Barrio La Calleja
author: Andres Gomez
image: /bogota/img/2021-04-22-OSM.png
---

Primer barrio de Bogotá completamente mapeado por Maptime Bogotá.
Para este actividad usamos las siguientes técnicas:

 * Fotografías con drone.
 * Fotografías a nivel de calle.
 * Trazas GPS.
 * Herramientas de calidad de datos.
 
Para las imágenes de drone, tomamos fotos a una altura de 120 metros, con la cámara apuntando hacia abajo (nadir) y se recorrió el barrio con control manual.
Esta no es la mejor manera, ya que la perpectiva de los edificios no queda bien capturada, y algunos lugares no se alcanzaron a captar.
En el drone, se puso una toma de fotos cada 2 segundos para capturar varias fotos; pero igualmente, por el vuelo manual, la velocidad no era constante durante el trayecto.
 
Una vez se descargaron las fotos, se generó una imagen por medio de OpenDroneMap, con la opción de [WebODM](https://www.opendronemap.org/webodm/) que se instaló.
Como no eran muchas imágenes, este tipo de instalación fue suficiente, como también el computador no requirió grandes capacidades de cómputo y terminó en pocos minutos (hubo un problema usandolo bajo Docker para Mac, por lo que se terminó usando directo bajo Linux Ubuntu.)
El resultado fue que generó un archivo TIF de casi 46 MB.

La imagen TIF, para compartirla con la comunidad, se publicó en OpenAerialMap.
Esta es [la imagen aerea del barrio La Calleja](https://map.openaerialmap.org/#/-74.04798030853271,4.712297883926474,15/square/03223211/604c3ffe5553510005076089?_k=d63imo).
Habiéndola publicado en este portal, el mapeo fue más fácil, ya que solo debemos referenciar la imagen como un Imagery adicional en formato TMS; y no cargarla directamente en JOSM ya que puede consumir mucha memoria.

Igualmente, se tomaron fotos a nivel de calle, montadas sobre un carro, con una actionCam apuntando al frente, otra apuntando atrás, y una 360 en la mitad.
Todas estas fotos fueron más de 10 mil, por lo que se subieron de manera bulk a Mapillary.
Aquí se pueden ver todas esas fotos: [https://www.mapillary.com/app/?focus=map&lat=4.712011402221506&lng=-74.05024101516284&z=14.819927381168846](https://www.mapillary.com/app/?focus=map&lat=4.712011402221506&lng=-74.05024101516284&z=14.819927381168846).

Durante el recorrido en el carro, se aprovechó y se capturó una traza GPX con el celular.
La traza quedó publicada aquí: [https://www.openstreetmap.org/user/AngocA/traces/3573909](https://www.openstreetmap.org/user/AngocA/traces/3573909)

Con todos estos datos en terreno, se comenzó a mapear con JOSM (Se hizo la transición a OpenWebStart, ya que Oracle Java no lo va a volver a incluir) y se fueron subiendo las contrucciones, vías y demás cosas que se identificaban.
Al principio, como íbamos a manejar un imagery nuevo, teníamos que estar seguros que estaba bien alíneado, por lo que usamos las trazas publicadas en OSM, más la que capturamos durante el trayecto en carro; sin embargo, la precisión de estas no es muy alta por usar la posición de un celular.
Como todo en el mundo de OSM, las características o features que no se conocías bien, fue bueno estudiarlas y evitar cometer errores.
En este caso estudiamos los hidrantes, la señales de tránsito de altura, lugares de venta de carros, parques de juego (play ground), entre otras.
Igualmente, para este mapeo, se usó la opción de edificio (construcción) y después se unían varios cuadros con Shift + j para darle la forma definitiva al edificio.

Finalmente, con todos estos datos ya cargados, le aplicamos las siguientes herramientas de calidad:

 * Validación de JOSM.
 * KeepRight.
 * Osmose.
 * OSM Inspector.

# Estado Inicial

# Resultados

Los resultados de este mapeo son estos:

## OpenStreetMap

[https://www.openstreetmap.org/#map=16/4.7124/-74.0496](https://www.openstreetmap.org/#map=16/4.7124/-74.0496)

![Barrio La Calleja en OpenStreetMap](/bogota/img/2021-04-22-OSM.png)

## Mapillary

[https://www.mapillary.com/app/?focus=map&lat=4.712011402221506&lng=-74.05024101516284&z=14.819927381168846](https://www.mapillary.com/app/?focus=map&lat=4.712011402221506&lng=-74.05024101516284&z=14.819927381168846)

![Barrio La Calleja en Mapillary](/bogota/img/2021-04-22-Mapillary.png)

## f4 demo

[https://demo.f4map.com/#lat=4.7108297&lon=-74.0513359&zoom=17&camera.theta=53.071&camera.phi=-9.271](https://demo.f4map.com/#lat=4.7108297&lon=-74.0513359&zoom=17&camera.theta=53.071&camera.phi=-9.271)

![Barrio La Calleja en f4](/bogota/img/2021-04-22-f4.png)

## Calidad de datos

[osmose](https://osmose.openstreetmap.fr/en/map/#zoom=16&lat=4.71214&lon=-74.0478&item=xxxx&level=1%2C2%2C3)

![Barrio La Calleja en osmose](/bogota/img/2021-04-22-Osmose.png)

[KeepRight](https://www.keepright.at/report_map.php?zoom=14&lat=-23.58791&lon=-46.65713)

![Barrio La Calleja en KeepRight](/bogota/img/2021-04-22-KeepRight.png)

# Estado inicial

* OpenStreetMap

![Barrio La Calleja en OSM](/bogota/img/2021-02-07-OSM.jpg)

* Mapillary

![Barrio La Calleja en Mapillary](/bogota/img/2021-02-07-Mapillary.jpg)

* Osmand

![Barrio La Calleja en Osmand](/bogota/img/2021-02-07-OsmAnd.jpg)

* Maps.me

![Barrio La Calleja en Maps.me](/bogota/img/2021-02-07-MAPSME.jpg)

# Lexiones aprendidas

* Hacer las tomas desde drone cuando está un poco nublado es lo mejor, ya que no se proyectan sombras.
* Con HiveMapper, se pueden tomar fotos desde drone. Esta utilidad genera el plan vuelo para usarlo desde Litchy. Esto lo usaremos en nuestro siguiente mapeo.
* Tener Ground Control Points para ubicar bien la posición en el mapa. Para eso, se van a hacer en tela y anclar con estacas de carpa de camping; además, la posición medianamente precisa, se puede obtener dejando el celular o GPS tracker un momento en el centro la cruz.
* En el carro, en vez de tener una cámara apuntando hacia atrás, se puede apuntar hacia la derecha para capturar las fachadas. Hacia atrás no se detectan muchas cosas y para eso es la captura de la foto 360. En cambio, hacia la derecha se pueden obtener los números de las direcciones o nombres de establecimientos.
* Es bueno hacer las cargas de fotos a Mapillary de noche, para evitar consumir el ancho de banda durante el día. Esto, por estar en tiempos de pandemia y teletrabajo, beneficia a la comunidad ya que no le impacta su actividad laboral, ya que la carga hacia Mapillary es intensiva.
* No intentar cargar un TIF o equivalente en JPG en JOSM, ya que consumirá toda la memoria de Java y se volverá demasiado lento.
* Los commits que se hagan a OSM, deben venir un un HashTag para poder asociar todos los commits de esta actividad. Algunos pueden ser #MaptimeBogota #NombreBarrio.
* Leer el wiki de OSM cuando hay un feature que no se le conocen los detalles.

# Faltantes

Con todo esto, ya se podría hacer un mapping party invitando a los residentes, y tomar los siguientes datos:

* Direcciones.
* Nombres de establecimientos.
* Altura de los edificios.
* Algún detalle de los pocos establecimientos de esta área, como especialidades médicas.
