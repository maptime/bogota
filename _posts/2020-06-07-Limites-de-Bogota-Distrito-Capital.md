---
layout: post
title: Límites de Bogotá Distrito Capital
author: Andres Gomez
---

Esta vez nos hemos encofado en los límites de Bogotá, específicamente los del distrito capital, los cuales colindan con otros departamentos (Nivel admnistrativo 6).
El objetivo de esta tarea ha sido ajustar el borde de los límites actuales a los que realmente son.
Para esto, nos apoyamos en los datos del IDECA, con las capas "Sector catastral" y "Localidad" para entender mejor los límites.
Igualmente, la capa de cuerpos de agua es muy útil, ya que muchos límites son rios o quebradas.
Por el lado de Sumapaz, debido a que es un páramo, ningún límite es exacto, por lo que los ajustamos a la geografía del lugar.

Además, se dejaron los límites de Bogotá independientes de otras características / features de OSM.
Por ejemplo, ya no se comparte el borde con el rio Bogotá, lo cual es inválido para un key de tipo Boundary.

Aquí les comparto el mapa de la relación de todos los bordes de Bogotá:

![Límites de Bogotá](/bogota/img/2020-06-07-limites-bogota.png)

Para ver la relación directamente en OSM, esta es la URL:
[https://www.openstreetmap.org/relation/1387968](https://www.openstreetmap.org/relation/1387968)

El Id de la relación es: 1387968

Para extraer la relación desde OverPasss Turbo: http://overpass-turbo.eu/s/UR8, la cual ejecuta el siguiente query:

    [out:json][timeout:25];
    (
      node["boundary"="administrative"]["admin_level"="6"]({{bbox}});
      way["boundary"="administrative"]["admin_level"="6"]({{bbox}});
      relation["boundary"="administrative"]["admin_level"="6"]({{bbox}});
    );
        out body;
    >;
    out skel qt;

Los límites de Bogotá son los siguientes. Comenzando desde la autopista norte en el sentido de la manecillas del reloj:

* Quebrada no determinada en OSM. (Quebrada Torca)
* Después son unas calles no pavimentadas sin nombre, pero muestran el delineamiento.
* Pasa por la mitad del IED La Aurora - Aurora Alta.
* Siguen calles sin nombre, las que están antes de una cantera. Más o menos el límite está entre líneas eléctricas.
* Siguen algunas vías sin nombre.
* Después es el borde de la montaña.
* Pasa por enfrente del Arboretto.
* Sigue el borde la montaña.
* Se aumenta después del camino del Meta.
* Sigue paralelo a las líneas eléctricas.
* Llega a alto de Patios.
* Ahí sigue en algunas calles del barrio San Luis, zona alta.
* Prosigue por un borde en la montaña.
* Comparte un tramo de la quebrada de Santos. (Quebrada Carrizal)
* Y sigue a lo largo del río Teusacá.
* Después se separa para seguir un tramo de la quebrada Turín. 
* Posteriormente cambia a bordear la calle San Isidro.
* Se vuelve a separar, para seguir una zona boscosa.
* Llega a compartir tramos del Camino Real, siendo una parte el camino entre Bogotá y Choachí.
* Después se dirigo hacia el alto Los Tunjos.
* Así sigue el borde la montaña, paralelo a unos acantilados, en el páramo Cruz Verde.
* Llega al alto de Cruz Verde.
* Comparte tramos con una vía.
* Sigue el borde de la montaña.
* Zigzaguea por las montañas, para llegar a una antenas.
* Pasa por la mitad de unas canteras.
* Sigue paralelo a una vía sin nombre.
* Después el borde es en un bosque, terminando el tramo en un acantilado.
* Prosigue en una calle.
* Pasa a ser el borde de un bosque.
* Comienza a saltar en varios acantilados, que son el borde de una montaña. Entre esos están Cerros de Bocagrande, El Pico de Aguila y Pico Buenavista.
* Sigue paralelo al rio Tabaco y después con el rio Pontezuela, para pasar al lado del río Pozo y llegar al rio Los Medios (Blanco). Posteriormente remontar por una quebrada, pero no tiene nombre (Quebrada Chibenchi) y llega al páramo de Sumapaz.
* Aquí bordea acantilados y las cimas de unas montañas.
* Llega a la quebrada Santa Rosa, y se bifurca en la quebrada Gallo, pasando al lado de la hoya el Cementario.
* Vuelve a bordear montañas y llega al alto de Torquita para pasar a la cuchilla de Los Frailes.
* Pasa cerca de la cuchilla Governador y cruza el alto Las Anuilas, la cuchilla Hermosura para llegar al paso del Meta.
* Llega a la parte más sur de Bogotá y vuelve hacia el norte por el occidente.
* Pasa al lado del batallón de alta montaña número 1.
* Pasa entre las corregimientos La Playa y La Unión.
* Toma el rio Sumapaz, pasando al lado de la vereda Las Vegas y la cuchilla del Pilar.
* Toma hacia el oriente entre montañas, por la quebrada San Antonio.
* Cruza el pantano de Andabobos (Quebrada Anabobos), para ir paralelo a la vía Usme - San Juan de Sumapaz, llegando a la cuchilla los encerrillos.
* Zigzaguea entre acantilados y lagunas para llegar al alto de Pasca. Y sigue de esta forma en zonas rurales, por el Rio Pilar
* Sigue pararelo a la quebrada Cucharita.
* Bordea Soacha, la calle 56A.
* Toma la quebrada La Muralla. (Quebrada Zanjón de la Muralla)
* Entra por la carrera 75C.
* Cambia a la carrera 75G para seguir por la diagonal 75F sur.
* Toma la calle 68B sur.
* Prosigue por la carrera 77C.
* Pasa por detrás de las carrera 77D.
* Sigue a lo largo de Pavimentos de Colombia S.A.
* Llega a Transmilenio.
* Sigue por la mitad de la cuadra entre la carrera 77H y carrera 13.
* Prosigue en la carrera 77G - carrera 24.
* Termina en la alameda el Porvenir.
* Toma la quebrada Tibanica - Canal Río Claro.
* Sigue por la carrera 77G.
* Sigue por el rio Tunjuelo.
* Llega al rio Bogotá.
* Antes del aeropuerto, entra a este, dejando unos cuerpos de agua a un costado.
* Justo después del aeropuerto vuelve al rio Bogotá.
* Finalmente, llega al canal Guaymaral, para cerrar el polígono con un cuerpo de agua que llega a la autopista (Canal Guaymaral Brazo Norte.
