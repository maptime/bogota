---
layout: post
title: Límites de Bogotá Urbana
author: Andres Gomez
---

Después de hacer los límites administrativos de Bogotá, los cuales se componen de parte urbana y rural, vamos a comenzar a delimitar la Bogotá Urbana.
Esta es la parte de la ciudad que muchos queremos ver en detalle, sin dejar a un lado la importancia de tener el páramo más grande del mundo a sur de nuestra ciudad.
En la parte urbana, correspondería al nivel 7 bajo la etiquete admin_level.

La silueta de esto lo dan la diferencia entre UPZ y UPR.
UPZ - Unidad de Planeamiento Zonal son agrupaciones de barrios en Bogotá, y en cierta forma determina la Bogotá Urbana.

Vamos a ir trabajando en el trazo de las UPZ por lo que la Bogotá Urbana irá tomando forma.
Por el momento es un trazo cercano entre los límites urbanos y rurales al sur de Bogotá.

![Límites de Bogotá Urbana](/bogota/img/2020-06-08-limites-bogota-urbana.png)

Para ver la relación directamente en OSM, esta es la URL:
[https://www.openstreetmap.org/relation/1387968](https://www.openstreetmap.org/relation/7426387)

El Id de la relación es: 7426387

Para extraer la relación desde OverPasss Turbo: [http://overpass-turbo.eu/s/URn](http://overpass-turbo.eu/s/URn), la cual ejecuta el siguiente query:

    [out:json][timeout:25];
    (
      node["boundary"="administrative"]["admin_level"="7"]({{bbox}});
      way["boundary"="administrative"]["admin_level"="7"]({{bbox}});
      relation["boundary"="administrative"]["admin_level"="7"]({{bbox}});
    );
        out body;
    >;
    out skel qt;

Los límites de Bogotá son los siguientes. Comenzando desde la autopista norte en el sentido de la manecillas del reloj:

* ToDo
