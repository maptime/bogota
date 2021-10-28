---
layout: post
title: Algunos queries para descargar datos en JOSM
author: Andres Gomez
---

Estos son unos queries para descargar en JOSM datos puntuales.

Descargar las vías de Bogotá que no comienzan con un nombre válido.

```
[out:xml][timeout:90];
area[name="Bogotá"][admin_level=7][boundary=administrative]->.searchArea;
(
  nwr["highway"~"trunk|primary|secondary|tertiary|residential"]["name"]["name"!~"^((Calle|Avenida Calle|Carrera|Avenida Carrera|Transversal|Avenida Transversal|Diagonal|Avenida Diagonal) [1-9][0-9]{0,2}[A-Z]{0,1}( Bis( [A-Z]){0,1}){0,1}( Este| Sur| Oeste| Norte){0,1}|Vía .*)$"](area.searchArea);
);
(._;>;);
out meta;
```

Descarga los elementos que tengan dirección, cuyo nombre de vía no sea válido.

```
[out:xml][timeout:90];
area[name="Bogotá"][admin_level=7][boundary=administrative]->.searchArea;
(
  nwr["addr:street"]["addr:street"!~"^(Calle|Avenida Calle|Carrera|Avenida Carrera|Transversal|Avenida Transversal|Diagonal|Avenida Diagonal) [1-9][0-9]{0,2}[A-Z]{0,1}( Bis( [A-Z]){0,1}){0,1}( Este| Sur| Oeste| Norte){0,1}$"](area.searchArea);
);
(._;>;);
out meta;
```
