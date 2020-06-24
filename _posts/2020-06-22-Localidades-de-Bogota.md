---
layout: post
title: Localidades de Bogotá
author: Andres Gomez
---

La ciudad de Bogotá está dividida en 20 localidades, las cuales están mapeadas con la etiqueta admin_level y un valor de 8.
Este es el mapa de Bogotá con todas sus localidades:

TODO ![Localidades Bogotá](/bogota/img/2020-06-22-localidades.png)

Para extraer las relaciones desde OverPasss Turbo: [http://overpass-turbo.eu/s/Vpu](http://overpass-turbo.eu/s/Vpu), la cual ejecuta el siguiente query:

    [out:json][timeout:25];
    (
      node["boundary"="administrative"]["admin_level"="8"]({{bbox}});
      way["boundary"="administrative"]["admin_level"="8"]({{bbox}});
      relation["boundary"="administrative"]["admin_level"="8"]({{bbox}});
    );
        out body;
    >;
    out skel qt;

Estas son las localidades con su relación respectiva:

* Usaquén
  * Referencia: 1
  * Id de la relación: 2214885
  * Relación en OSM [https://www.openstreetmap.org/relation/2214885](https://www.openstreetmap.org/relation/2214885).
* Chapinero
  * Referencia: 2
  * Id de la relación: 1379547
  * Relación en OSM [https://www.openstreetmap.org/relation/1379547](https://www.openstreetmap.org/relation/1379547).
* Santa Fe
  * Referencia: 3
  * Id de la relación: 4740232
  * Relación en OSM [https://www.openstreetmap.org/relation/4740232](https://www.openstreetmap.org/relation/4740232).
* San Cristóbal
  * Referencia: 4
  * Id de la relación: 4740231
  * Relación en OSM [https://www.openstreetmap.org/relation/4740231](https://www.openstreetmap.org/relation/4740231).
* Usme
  * Referencia: 5
  * Id de la relación: 4740233
  * Relación en OSM [https://www.openstreetmap.org/relation/4740233](https://www.openstreetmap.org/relation/4740233).
* Tunjuelito
  * Referencia: 6
  * Id de la relación: 2216689
  * Relación en OSM [https://www.openstreetmap.org/relation/2216689](https://www.openstreetmap.org/relation/2216689).
* Bosa
  * Referencia: 7
  * Id de la relación: 4740227
  * Relación en OSM [https://www.openstreetmap.org/relation/4740227](https://www.openstreetmap.org/relation/4740227).
* Kennedy
  * Referencia: 8
  * Id de la relación: 4740229
  * Relación en OSM [https://www.openstreetmap.org/relation/4740229](https://www.openstreetmap.org/relation/4740229).
* Fontibón
  * Referencia: 9
  * Id de la relación: 2216630
  * Relación en OSM [https://www.openstreetmap.org/relation/2216630](https://www.openstreetmap.org/relation/2216630).
* Engativá
  * Referencia: 10
  * Id de la relación: 2214883
  * Relación en OSM [https://www.openstreetmap.org/relation/2214883](https://www.openstreetmap.org/relation/2214883).
* Suba
  * Referencia: 11
  * Id de la relación: 2214884
  * Relación en OSM [https://www.openstreetmap.org/relation/2214884](https://www.openstreetmap.org/relation/2214884).
* Barrios Unidos
  * Referencia: 12
  * Id de la relación: 2214882
  * Relación en OSM [https://www.openstreetmap.org/relation/2214882](https://www.openstreetmap.org/relation/2214882).
* Teusaquillo
  * Referencia: 13
  * Id de la relación: 2216632
  * Relación en OSM [https://www.openstreetmap.org/relation/2216632](https://www.openstreetmap.org/relation/2216632).
* Los Mártires
  * Referencia: 14
  * Id de la relación: 2216631
  * Relación en OSM [https://www.openstreetmap.org/relation/2216631](https://www.openstreetmap.org/relation/2216631).
* Antonio Nariño
  * Referencia: 15
  * Id de la relación: 2216654
  * Relación en OSM [https://www.openstreetmap.org/relation/2216654](https://www.openstreetmap.org/relation/2216654).
* Puente Aranda
  * Referencia: 16
  * Id de la relación: 2216655
  * Relación en OSM [https://www.openstreetmap.org/relation/2216655](https://www.openstreetmap.org/relation/2216655).
* La Candelaria
  * Referencia: 17
  * Id de la relación: 166430030
  * Relación en OSM [https://www.openstreetmap.org/relation/166430030](https://www.openstreetmap.org/relation/166430030).
* Rafael Uribe Uribe
  * Referencia: 18
  * Id de la relación: 4740230
  * Relación en OSM [https://www.openstreetmap.org/relation/4740230](https://www.openstreetmap.org/relation/4740230).
* Ciudad Bolivar
  * Referencia: 19
  * Id de la relación: 4740228
  * Relación en OSM [https://www.openstreetmap.org/relation/4740228](https://www.openstreetmap.org/relation/4740228).
* Sumapaz
  * Referencia: 20
  * Id de la relación: 5579632
  * Relación en OSM [https://www.openstreetmap.org/relation/5579632](https://www.openstreetmap.org/relation/5579632).
