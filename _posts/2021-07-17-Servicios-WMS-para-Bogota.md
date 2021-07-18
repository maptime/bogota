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
![Pagina del IDECA](/bogota/img/2021-07-17-2-IDECA.png)

Aquí nos muestra todos los servicios web que ofrece esa página (https://www.ideca.gov.co/buscador).
Para buscar directamente la foto aerea, escribimos lo siguiente en el campo de búsqueda: ortofoto
![Buscador IDECA](/bogota/img/2021-07-17-3-IDECA-buscador.png)

Ahí nos mostrará todas las ortofotos disponibles.
Al momento de escribir esto, la más reciente es del 2014.
(https://www.ideca.gov.co/recursos/mapas/ortoimagen-bogota-dc-2014):
![Ortofotos](/bogota/img/2021-07-17-4-ortofotos.png)

Una vez le damos click en descargar (la flecha hacia abajo), nos dirigirá a una URL como la siguiente URL: https://serviciosgis.catastrobogota.gov.co/arcgis/services/imagenes/Ortho2014/MapServer/WMSServer?
Podemos copiar la URL hasta el signo de pregunta.
![URL](/bogota/img/2021-07-17-5-URL.png)

Con la URL copiada, podemos irnos a JOSM y buscamos la opción Preferencias.
![JOSM](/bogota/img/2021-07-17-6-josm.png)
![Preferencias JOSM](/bogota/img/2021-07-17-7-preferencias.png)

Dentro de la ventana de preferencias buscamos la sección de Imagery.
![Imagery](/bogota/img/2021-07-17-8-imagery.png)

Ahí podemos ver unos botones al lado derecho que indican el tipo de imagery que queremos. Para este caso seleccionaos WMS, y nos abrirá una neuva ventana.
![WMS](/bogota/img/2021-07-17-9-WMS.png)


En la nueva ventana, pegamos la URL en el campo 2, seguido de clikc sobre get Layers.
![Get Layers](/bogota/img/2021-07-17-10-getLayers.png)

Esto nos mostrará la lista de capas disponibles. Para el caso de la Ortofoto solo habrá la que hayamos escogido.
![Layers](/bogota/img/2021-07-17-11-layers.png)

En el último campo le debemos poner un nombre.
Por defecto pone la URL, podemos cambiarla por algo más explícito.
IMPORTANTE: Como nombre recomendamos poner algo así: IDECA Ortofoto 2014.
Con un nombre como este, automáticamente aparecerá en el campo de Fuentes al hacer commit en OSM.
![Nombre por defecto](/bogota/img/2021-07-17-12-nombre.png)
![Nuevo nombre](/bogota/img/2021-07-17-13-nuevoNombre.png)

Debido a que estamos usando una fuente de datos que ofrece el IDECA, es importante reconocerlos en nuestros cambios.
Referenciar la propiedad intelectual es vital en OSM.

Salimos de las prefencias.
![Salir de preferencias](/bogota/img/2021-07-17-14-salir.png)

En JOSM selecccionamos la imagery del IDECA.
![Selccionar imagery](/bogota/img/2021-07-17-15-imagery.png)

Finalmente, ya podemos ver la ortofoto en JOSM
![Ortofoto 2014](/bogota/img/2021-07-17-16-josm.png)

Podemos ver mejores detalles de Bogotá, por ejemplo la glorieta de la calle 65 con carrera 50 (donde está el nombre Bogotá en el mapa).
![Detalle Ortofoto 2014](/bogota/img/2021-07-17-17-detalle.png)

# Instituco Geográfico Agustín Codazzi - IGAC

De manera similar al WMS del IDECA, buscamos en Google: datos abiertos igac
![Google](/bogota/img/2021-07-17-1-IGAC-google.png)

En la página del IGAC vemos todo lo que ofrece como servicios web (https://geoportal.igac.gov.co/contenido/geoservicios):
![Servicios Web del IGAC](/bogota/img/2021-07-17-2-IGAC-web services.png)

Por ejemplo, si tomamos la cartografía Base Escala 1:100000, obtendremos la siguiente URL:
http://gw-geoportal-test.igac.gov.co/cartografia100k/service?
![URL](/bogota/img/2021-07-17-3-IGAC-URL.png)

Con esa URL vamos a preferencias de JOSM, y en imagery adicionamos un WMS:
![Imagery](/bogota/img/2021-07-17-4-IGAC-imagery.png)

Escogemos cualquiera de las capas. En nuestro caso fue Administrativo Punto.
![Layers](/bogota/img/2021-07-17-5-IGAC-layers.png)

Para eso ponemos un nombre apropriado como nombre de capa.
![Nombre de la capa](/bogota/img/2021-07-17-6-IGAC-name.png)

Particularmente esta capa tiene letras negras, por lo que será necesario cambiar el color de fondo de JOSM.
![Color de fondo](/bogota/img/2021-07-17-7-IGAC-backgroundColor.png)

Con eso ya se podrán ver los valores cuando se hace bastante zoom.
![Datos](/bogota/img/2021-07-17-8-IGAC-data.png)

# Parques nacionales

De manera similar se puede hacer para los WMS de Parques Nacionales.
Buscando en Google: geoservicios parques nacionales de colombia

# Referencias:
* Web Map Service - https://es.wikipedia.org/wiki/Web_Map_Service
