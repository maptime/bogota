#Información a recoger de cada construcción

Las construcciones en OSM se mapean principalmente con la llave Building, pero puede tener diferentes valores.
Por este motivo es necesario conseguir la siguiente información para que el mapeo sea rico en información.

Antes de comenzar, es necesario explicar que el uso original para que se construyó el edificio puede que no sea el uso actual.

* Tipo de construcción https://wiki.openstreetmap.org/wiki/Key:building:
  * Es un edificio, torre - appartments https://wiki.openstreetmap.org/wiki/Tag:building%3Dapartments,
  * es una casa (junto a otra construcción) - house,
  * es una casa separada sin muros adyacentes a otras construcciones - detached,
  * es una construcción residencial que no se sabe qué es - residential,
  * es un edificio que no es residencial - yes,
  * es otro tipo de edificio
    * Hospedaje: hotel, granja, dormitorio/residencia estudiantil
    * Comercial: Industrial, Bodega
    * Servicios: Catedral, capilla, iglesia, mesquita, templo, sinagoga, cívico (genérico), hospital, colegio, estadio, estación de tren, transporte, universidad, público 
    * Otros
* Uso de la construccion, si no es el mismo uso por el que se construyó originalmente
https://wiki.openstreetmap.org/wiki/Key:building:use
* Material de la fachada: ladrillo, vidrio, vidrio reflectivo, piedra, cemento, bahareque
https://wiki.openstreetmap.org/wiki/Key:building:material
* Material del techo: Eternit, concreto, vidrio, pasto (techo verde), gravilla, plantas, tejas, tela/shadecloth, pizarra, piedra, paja, madera.
https://wiki.openstreetmap.org/wiki/Key:roof:material
* Estilo de la arquitectura: Colonial, moderno
* Niveles https://wiki.openstreetmap.org/wiki/Key:building:levels
* Altura https://wiki.openstreetmap.org/wiki/Key:height
* Entradas: principal, de servicio, de emergencia, solo salida, de casa https://wiki.openstreetmap.org/wiki/Key:entrance
  * Tipo de puerta: pivote, deslizante, giratoria, elevadiza, sin puerta (arco). 
* Dirección https://wiki.openstreetmap.org/wiki/Key:addr
  * Completa (full): Calle 118 # 6A - 01
  * Número (housenumber): La intersección y la distancia. En el ejemplo: 6A-01
  * Calle (street): La carrera X o calle X. En el ejemplo: Calle 118 
  * Cantidad de apartamentos https://wiki.openstreetmap.org/wiki/Key:addr:flats
  * Código postal: 110111 http://visor.codigopostal.gov.co/472/visor/#
  * Barrio (suburb): Usaquén
  * Localidad (district): Usaquén 
  * Ciudad: Bogotá
  * Departamento (state): Distrito Capital
  * Pais: CO

Otras cosas que se pueden mapear

* Aparte el servicio https://wiki.openstreetmap.org/wiki/Key:amenity
* Barreras: muros/pared, murallas, rejas, pasamanos, zardineles https://wiki.openstreetmap.org/wiki/Key:barrier
