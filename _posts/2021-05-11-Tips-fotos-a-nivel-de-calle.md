---
layout: post
title: Tips para fotos a nivel de calle
author: Andres Gomez
---

Esta es una nota corta de cómo utilizar una cámara como la LG 360 (ya descontinuada), para tomar fotos 360.
Se debe configurar la cámara con el celular, para poder "programarla".
Para esto, hay que conectar el celular por wifi y bluetooth, y después la aplicación se conectará "fácilmente"; de lo contrario puede ser tedioso.

Se debe programar para que tome fotos cada 2 segundos. Sería ideal que tuviera menos tiempo, pero esta cámara no es como una ActionCam.

Después de varias pruebas, no recomiendo usar el posicionamiento GPS del celular, con el que se puede configurar.
Esto ocasiones que las fotos no tengan una periodicidad constante, sino que empieza a tener latencias, dañando la secuencia de fotos.

En cambio, es mejor capturar una traza GPX en el celular y después hacer la correspondencia entre fotos y traza.
Para esto se puede usar JOSM, donde se abren todas las fotos, y se le da click derecho sobre Geotagged Images.
Ahí se le dice Correlate to GPX y se selecciona la traza GPX que hayamos capturado (Osmand o Open GPX Tracker) y ya tengamos en el computador.

Finalmente, para guardar la posición en las fotos se requiere el plugin Photo Geotaggin: https://wiki.openstreetmap.org/wiki/JOSM/Plugins/Photo_Geotagging
Donde al dar click derecho sober las fotos se puede seleccionar Write Coordinates to image header.

Con esto, ya se podrá subir a Mapillary u OpenStreetCam.
