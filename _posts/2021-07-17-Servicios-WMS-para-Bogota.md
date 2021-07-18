---
layout: post
title: Servicios WMS disponibles para Bogotá
author: Andres Gomez
---

La información que a continuación explicó, me la compartió el usuario JuanMelo.
Varias de las instituciones geográficas o de temas relacionados, comparten su información de manera OpenData para que la use la comunidad.
Estos servicios web ofrecen información abierta de Bogotá, donde la información es compatible con la licencia de OpenStreetMap.
Los servicios web son de mapas con temáticas puntuales.

# Catastro IDECA

Para comenzar, podemos buscar en Google: geoservicios IDECA:
![Búsqueda en Google](/bogota/img/2021-07-17-1-google.png)

Una vez estamos en la página del IDECA (https://www.ideca.gov.co/recursos/mapas/mapa-de-referencia-para-bogota-dc), escogemos la opción "Buscador".
![Barrio La Calleja en OpenStreetMap](/bogota/img/2021-04-22-OSM.png)
![Pagina del IDECA](/bogota/img/2021-07-17-2-IDECA.png)

Aquí nos muestra todos los servicios web que ofrece esa página (https://www.ideca.gov.co/buscador).
Para buscar directamente la foto aerea, escribimos lo siguiente en el campo de búsqueda: ortofoto
![Buscador IDECA](/bogota/img/2021-07-17-3-IDECA-buscador.png)

Una vez le damos click en descargar (la flecha hacia abajo), nos dirigirá a una URL como la siguiente (https://www.ideca.gov.co/recursos/mapas/ortoimagen-bogota-dc-2014):
URL: https://serviciosgis.catastrobogota.gov.co/arcgis/services/imagenes/Ortho2014/MapServer/WMSServer?
Podemos copiar la URL hasta el signo de pregunta.
![Ortofotos](/bogota/img/2021-07-17-4-ortofotos.png)

Con la URL copiada, podemos irnos a JOSM y buscamos la opción Preferencias.
![Preferencias JOSM](/bogota/img/2021-07-17-5-preferencias.png)

Dentro de la ventana de preferencias buscamos la sección de Imagery.
![Imagery](/bogota/img/2021-07-17-6-imagery.png)

Ahí podemos ver unos botones al lado derecho que indican el tipo de imagery que queremos. Para este caso seleccionaos WMS, y nos abrirá una neuva ventana.
![WMS](/bogota/img/2021-07-17-7-WMS.png)


En la nueva ventana, pegamos la URL en el campo 2, seguido de clikc sobre get Layers.
![Get Layers](/bogota/img/2021-07-17-8-getLayers.png)

Esto nos mostrará la lista de capas disponibles. Para el caso de la Ortofoto solo habrá la que hayamos escogido.
![Layers](/bogota/img/2021-07-17-9-layers.png)

En el último campo le debemos poner un nombre.
Por defecto pone la URL, podemos cambiarla por algo más explícito.
IMPORTANTE: Como nombre recomendamos poner algo así: IDECA Ortofoto 2014.
Con un nombre como este, automáticamente aparecerá en el campo de Fuentes al hacer commit en OSM.

Debido a que estamos usando una fuente de datos que ofrece el IDECA, es importante reconocerlos en nuestros cambios.
Referenciar la propiedad intelectual es vital en OSM.

Finalmente, ya podemos ver la ortofoto en JOSM
![Ortofoto 2014](/bogota/img/2021-07-17-10-josm.png)

# Instituco Geográfico Agustín Codazzi - IGAC


#

Referencias:
* Web Map Service - https://es.wikipedia.org/wiki/Web_Map_Service
