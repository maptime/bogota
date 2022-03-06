---
layout: post
title: Resultado del mapping party de Nicolás de Federmán, Bogotá
author: Andres Gomez
---

Como parte del evento mundial del día de los datos abiertos - OpenDataDay, se hizo una actividad de mapeo en el barrio Nicolás de Federmán, en Bogotá.
Sin embargo, el clima no fue nuestro aliado y la lluvia fue muy intensa durante la tarde y noche.

Pero esto no impidió que hiciéramos el evento, y que la comunidad participara.
Hubo varios asistentes, y el mapa del barrio se mejoró gracias a la aplicación StreetComplete.

Por medio de esta aplicación se adicionaron detalles de las construcciones, como el tipo de edificio, la dirección, la altura; igualmente, las superficies de los andenes y calles.

Para poder lograr esto, que StreetComplete generara tantas preguntas, se habìa preparado el terreno previamente gracias a la ortofoto del IDECA de 2017, y se dibujaron los polígonos de cada casa u edificio.
Igualmente, se arreglaron las calles y se dibujaron los andenes para que estuvieran conectados por cruces.
Se ajustaron los parques y algunos establecimientos conocidos del barrio.

Este es el mapa de lo trabajado: [https://www.openstreetmap.org/#map=17/4.64790/-74.08197](https://www.openstreetmap.org/#map=17/4.64790/-74.08197)

Por medio de este query en Overpass Turbo se puede descargar todo el barrio, y trabajar en el futuro en JOSM:

```
[out:json][timeout:25];
   area[name="Nicolas de Federman"][admin_level=10]->.searchArea;
   (
     nwr
   (area.searchArea);
<;
   ); out meta;
```

Redes sociales

* [instagram](https://www.instagram.com/p/Cav-FvjOs6N/)
* [twitter](https://twitter.com/MaptimeBogota/status/1500336861524500481?s=20&t=rlYJ79hlaE1izdMNlOYehQ)
