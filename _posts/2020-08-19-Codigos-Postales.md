---
layout: post
title: Códigos Postales de Bogotá
author: Andres Gomez
---

El Miniterio de la Tecnología de Información y Comunicaciones - MinTIC definió, por medio de 7/24 - Correo postal, unos códigos postales en todas Colombia.
Dichos códigos postales son un conjunto de áreas que dividen el territorio colombiano, para facilitar la mensajería.
Los límites de dichos códigos postales han sido publicados como datos abiertos.

Aquí presentamos los códigos postales que hay en OpenStreetMap.

Se creó una relación abuelo para contener los códigos postales de todas las localidades, cuyo id es:
Para cada localidad, se creó una relación que contiene los códigos postales de dicha área, así:

* 1 - Códigos postales localidad de Usaquén: 
* 2 - Códigos postales localidad de Chapinero: 
* 3 - Códigos postales localidad de Santa Fe: 
* 4 - Códigos postales localidad de San Cristobal: 
* 5 - Códigos postales localidad de Usme: 
* 6 - Códigos postales localidad de Tunjuelito: 
* 7 - Códigos postales localidad de Bosa: 
* 8 - Códigos postales localidad de Kennedy: 
* 9 - Códigos postales localidad de Fontibón: 
* 10 - Códigos postales localidad de Engativá: 
* 11 - Códigos postales localidad de Suba: 
* 12 - Códigos postales localidad de Barrios Unidos: 
* 13 - Códigos postales localidad de Teusaquillo: 
* 14 - Códigos postales localidad de Los Mártires: 
* 15 - Códigos postales localidad de Antonio Nariño: 
* 16 - Códigos postales localidad de Puente Aranda: 
* 17 - Códigos postales localidad de La Candelaria: 
* 18 - Códigos postales localidad de Rafael Uribe Uribe: 
* 19 - Códigos postales localidad de Ciudad Bolivar: 
* 20 - Códigos postales localidad de Sumapaz: 

Para extraer las relaciones desde OverPasss Turbo: [http://overpass-turbo.eu/s/XdD](http://overpass-turbo.eu/s/XdD), la cual ejecuta el siguiente query:

    [out:json][timeout:25];
    // gather results
    (
      // query part for: “boundary=administrative”
      node["boundary"="postal_code"]({{bbox}});
      way["boundary"="postal_code"]({{bbox}});
      relation["boundary"="postal_code"]({{bbox}});
    );
    // print results
    out body;
    >;
    out skel qt;
