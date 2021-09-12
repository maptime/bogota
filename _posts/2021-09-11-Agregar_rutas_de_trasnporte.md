---
layout: post
title: Agregar rutas de transporte.
author: Andres Gomez
---

Estas son las memorias del evento organizado el 11 de septiembre, donde nuestro invitado principal fue Leonardo Gutiérrez - LeoGuti de la organización Trufi.
La página de Trufi es: https://www.trufi-association.org/ y el correo de Leo es: leonardo.gutierrez@trufi-association.org.

Además, hubo otros invitados como:

* Newton Davis - https://mobilitydata.org/
  * newton@mobilitydata.org
* Samuel Rioja - Trufi Association
 
Newton nos habló un poco de las especificaciones:

* El GTFS: [https://en.wikipedia.org/wiki/General_Transit_Feed_Specification](https://en.wikipedia.org/wiki/General_Transit_Feed_Specification)
* El GBFS: [https://github.com/NABSA/gbfs](https://github.com/NABSA/gbfs)

Finalmente, nos invitó a participar en:

* MobilityData 101
* Audience: every industry stakeholder who wants to learn more about us
* Date: September 22, 2021
* Time: 09:00 CEST, 11:00 EDT, and 16:00 PDT
* Language: English
* Price: free of charge
* Registration [http://bit.ly/MobilityData101](http://bit.ly/MobilityData101)

Leonardo nos explicó cómo agregar rutas de transporte y nos mostró un video de lo que se puede hacer con esas rtuas de transporte:
Public Transport in Nouakchott, Mauritania - Mapped by Trufi | Trufi Association [https://youtu.be/ydzOe3z0zC0](https://youtu.be/ydzOe3z0zC0)

Leonardo también nos explicó cómo usar JOSM desde su descarga hasta su uso avanzado para el mapeo de rutas.
Se descarga de aquí: [https://josm.openstreetmap.de/wiki/Download](https://josm.openstreetmap.de/wiki/Download).
Para aprender más de JOSM [https://learnosm.org/es/](https://learnosm.org/es/).
Alex nos compartió un instructivo de cómo instalar JOSM [https://wiki.openstreetmap.org/wiki/ES:JOSM/Instalaci%C3%B3n](https://wiki.openstreetmap.org/wiki/ES:JOSM/Instalaci%C3%B3n)

Samuel nos compartió una herramienta para personalizar JOSM para el mapeo de rutas: [https://github.com/trufi-association/routemapping_josmconfig](https://github.com/trufi-association/routemapping_josmconfig).

Para mapear rutas en terreno, Leonardo con recomendó esta aplicación, la cual captura trazas GPX: [https://play.google.com/store/apps/details?id=net.osmtracker](https://play.google.com/store/apps/details?id=net.osmtracker).
Un manual de cómo usarla está aquí: [https://learnosm.org/es/mobile-mapping/osmtracker/](https://learnosm.org/es/mobile-mapping/osmtracker/).
Una forma de personalizar OSM Tracker para captura de datos de transporte: [https://github.com/labexp/osmtracker-android-layouts/blob/master/layouts/transporte_publico/README.md](https://github.com/labexp/osmtracker-android-layouts/blob/master/layouts/transporte_publico/README.md).

Cuando se cambia a modo Experto (ícono de Albert Einstein) en JOSM, se puede descargar por tipo de feature.
En este caso, Leonardo solo descarga las vías con este query:

```
[out:xml][timeout:90][bbox:{{bbox}}];
(
  nwr["highway"];
);
(._;>;);
out meta;
```

Para alinear las vías a trazas GPX, Leonardo nos recomienda usar el Heatmap de Strava.
Para configurarlo en OSM se puede seguir este tutorial: [https://erickdeoliveiraleal.medium.com/tutorial-strava-openstreetmap-josm-or-id-2e2003f4aea3](https://erickdeoliveiraleal.medium.com/tutorial-strava-openstreetmap-josm-or-id-2e2003f4aea3).
Esta configuración hay que renovarla cada 2 semanas.

Otra forma de dibujar rutas es por medio del mapa de trayecto.
Entonces, Leonardo nos recomienda cargar la imagen directamente en OSM por medio del plugin PicLayer: [https://wiki.openstreetmap.org/wiki/JOSM/Plugins/PicLayer](https://wiki.openstreetmap.org/wiki/JOSM/Plugins/PicLayer
)

Para mapear una ruta en OSM, se maneja una [relación](https://wiki.openstreetmap.org/wiki/ES:Relaciones).

Para cortar las vías a medida que se mapea, se puede oprimir la letra p de [Split Way](https://josm.openstreetmap.de/wiki/Help/Action/SplitWay).

El objetivo es mapear una ruta como se explica aquí [https://wiki.openstreetmap.org/wiki/Tag:route%3Dbus](https://wiki.openstreetmap.org/wiki/Tag:route%3Dbus), debe tener de manera general las siguientes etiquetas:

* from: Zona desde donde comienza la ruta
* to: Zona a donde termina la ruta
* name: nombre de la ruta, donde se puede incluir el código de la ruta.
* operator: la empresa que usa esa ruta
* public_transportation:version: poner 2, que es la versión actual
* ref: el código de la ruta
* route: bus
* type: route

Si se tienen dudas acerca de las rutas de manera general, se puede visitar [https://wiki.openstreetmap.org/wiki/Relation:route](https://wiki.openstreetmap.org/wiki/Relation:route).

En el ejemplo realizado se mapeó una ruta de Yopal, Casanare, la cual se puede consultar en: [http://www.yopal-casanare.gov.co/tema/normatividad](http://www.yopal-casanare.gov.co/tema/normatividad
).

Un ejemplo de una ruta mapeada en Mauritania se puede ver en: [https://www.openstreetmap.org/relation/12433026#map=13/18.1147/-15.9975&layers=T](https://www.openstreetmap.org/relation/12433026#map=13/18.1147/-15.9975&layers=T).

Como las rutas tienen intervalos, estos se deben mapear según esto [https://wiki.openstreetmap.org/wiki/Key:interval](https://wiki.openstreetmap.org/wiki/Key:interval).

Cuando la ruta va, y después vuelve, entonces se debe hacer un master route siguiendo esto: [https://wiki.openstreetmap.org/wiki/Relation:route_master](https://wiki.openstreetmap.org/wiki/Relation:route_master).

Una vez mapeadas las rutas, podemos usarlas en: [https://github.com/trufi-association/trufi-backend-demo](https://github.com/trufi-association/trufi-backend-demo).

Finalmente, Leonardo nos invita a postular nuestras ciudades en Trufi, llenando este artículo: https://forms.gle/i4QMdJ37vmX26Wy38

Entre los participantes hubo personas de:

* Manor, Texas, USA.
* Chicago, Ilinois, USA.
* Hamburgo, Alemania.
* Toluca, México.
* Lima, Peru.
* Cochabamba, Bolivia.
* Alajuela, Costa Rica.
* Heredia, Costa Rica.
* Barquisimeto, Venezuela.
* Popayán, Cauca, Colombia.
* Cúcuta, Santander, Colombia.
* Yopal, Casanare, Colombia.
* Duitama, Boyacá, Colombia.
* Bogotá, DC., Colombia.

Estos datos se obtuvieron por medio de slido.com, código 063 734.

Entre los participantes tuvimos a:

* Doris Ruiz.
* Sandra Hernández.
* Luis Ortiz.
* Alex Mayorga.
* @kaxtillo.
* Freddy Jiménez.
* Wilmer Osario.
* Rafael Isturiz.
* Jaime Mejía.
* Jaime Gutiérrez.
* Gabriel.
* Josselin Guzmán.
* Harry Chuquicusma.
* Leonardo Pinzón N.
* Julio M.

Quienes son contribuidores principiando, intermedios y avanzados a OSM.
