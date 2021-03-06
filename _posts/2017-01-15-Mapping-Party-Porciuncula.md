---
layout: event
category: event
title: Meetup para mapear la Porciúncula
rsvp: https://www.meetup.com/Maptime-Colombia-OSM/events/236927128/
---

En esta ocasión vamos a mapear la zona de la Porcíuncula, la calle 72 y la carrera 11, donde ya hay varios 
datos en OSM, por lo que vamos a actualizarlos y corregir los edificios.

Este Mapping party se realizará el sábado 21 de enero de 2017 a las 9:00 am.
Nuestro punto de encuentro será al lado de la iglesia de la Porciúncula, donde se robaron la estatua de
bronce de uno de los animales de San Francisco de Asis.
Ahí nos podrás encontrar fácilmente. Igualmente, tendremos un botón con el logo de OpenStreetMap.

Si no puedes asistir presencialmente, nos puedes ayudar remotamente una vez hayamos recogido los datos.
Aquí publicaremos los field papers, trazas, fotos y demás información para hacer el mapeo en OSM.

Organizador: Andrés Gómez (+57 316 621 40 32, Twitter: [@angoca](http://twitter.com/angoca),
WhatsApp [Grupo](https://chat.whatsapp.com/Is8kErwoFDg0SwtyWcjD0o)).

-----

## Preparación:

- [X] Definir el punto de encuentro a las 9
- [ ] Definir el punto de mapeo a las 10:15
- [ ] Crear el espacio en github para las fotos y GPX recogidos
- [ ] Pasar en bici tomando fotos para Mapillary
- [ ] Subir las fotos a Mapillary
- [X] Preparar el atlas de field papers http://fieldpapers.org/atlases/3ciatg21
- [ ] Imprimir el atlas
- [ ] Bajar la zona de OSM para tenerla local en caso de falta de Internet

-----

A continuación, la descripción de los datos que vamos a recoger.

## Datos a recoger:

* Edificios http://wiki.openstreetmap.org/wiki/Key:building
  * Forma, area
  * Cantidad de niveles (pisos) http://wiki.openstreetmap.org/wiki/Key:building:levels
  * Dirección http://wiki.openstreetmap.org/wiki/Key:addr
  * Altura si se tiene el metro digital http://wiki.openstreetmap.org/wiki/Key:height
* Tiendas http://wiki.openstreetmap.org/wiki/Key:shop
* Restaurantes, bares, cafés, comida rápida, pub http://wiki.openstreetmap.org/wiki/Tag:amenity%3Drestaurant, http://wiki.openstreetmap.org/wiki/Tag:amenity%3Dbar, 
  * Horarios http://wiki.openstreetmap.org/wiki/Key:opening_hours
* Bolardos http://wiki.openstreetmap.org/wiki/Tag:barrier%3Dbollard
  * Material
* Faros http://wiki.openstreetmap.org/wiki/Tag:highway%3Dstreet_lamp
* Canecas http://wiki.openstreetmap.org/wiki/Tag:amenity%3Dwaste_basket
* Zonas verdes, jardines http://wiki.openstreetmap.org/wiki/Tag:leisure%3Dgarden
* Esculturas http://wiki.openstreetmap.org/wiki/Key:artwork_type
* Placas conmemorativas http://wiki.openstreetmap.org/wiki/Key:memorial
* Monumentos http://wiki.openstreetmap.org/wiki/Tag:historic%3Dmemorial
* Arboles http://wiki.openstreetmap.org/wiki/Tag:natural%3Dtree
* Puntos geodésicos http://wiki.openstreetmap.org/wiki/Tag:man_made%3Dsurvey_point
* Andenes http://wiki.openstreetmap.org/wiki/Sidewalks
* Peldaños http://wiki.openstreetmap.org/wiki/Tag:highway%3Dsteps
  * Cantidad
* Semáforos https://wiki.openstreetmap.org/wiki/Tag:highway%3Dtraffic_signals
* Cruces peatonales https://wiki.openstreetmap.org/wiki/Tag:highway%3Dcrossing
* Paraderos https://wiki.openstreetmap.org/wiki/Tag:highway%3Dbus_stop
* Ciclorutas

## Fotos a tomar:

* De cada inmueble, de frente para ver la estructura. Puede ser desde la acera del frente. Si es muy grande, pueden ser varias fotos.
* De los detalles, como árboles, canecas, bolados, postes, para saber dónde están ubicados. Por eso toca tomar el contexto.

## Herramientas para mapeo

* División de trabajo http://mapcraft.nanodesu.ru/
* FieldPapers
* GPS de celulares
  * Android: OSM tracker https://play.google.com/store/apps/details?id=me.guillaumin.android.osmtracker&hl=en
  * iPhone:
  * Windows:
* Fotos georeferenciadas
  * Fotos de celulares o cámaras con GPS
  * Mapillary http://www.mapillary.com/
* Encuesta de los datos a conseguir de las construcciones: https://github.com/maptime/bogota/blob/master/src/doc/2016-05-07/Informacion-Construcciones.md

## Técnicas

* Cuando inicien una captura, mover el celular en las tres direcciones (adelante-atrás, izquierda-derecha, rotación en ambos sentidos). Esto mejorará la precisión para iniciar la captura.
* Comenzar capturas frecuentemente, cada 15 minutos es un buen valor. Esto permite tener más trazas y algunas veces con mejor precisión.
* Para capturar puntos, se recomienda recorrer el objeto alrededor para captura una mejor ubicación. Con esto la traza tendrá para trackpoints y lo ubicará mejor. Por ejemplo si es un árbol, acercarse al árbol y caminar alrededor de él mientras se crea la nota.
* Para capturar un área, se recomienda caminar sobre el borde de esta. Por ejemplo si es una zona verde, caminar en las partes limítrofes de la zona verde, y así la traza GPX capturará los puntos sobre esta, de manera que cuando se vayan a mapear, los puntos corres
* Pasar varios dispositivos GPS o varias personas con su celular por el mismo lugar para así tener una mayor precisión.

