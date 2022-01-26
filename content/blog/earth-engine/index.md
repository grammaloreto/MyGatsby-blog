---
title: Google Earth Engine (GEE) para investigación remota
date: "2021-12-13T23:46:37.121Z"
description: Los satélites u otros objetos de detección remota generan una enorme cantidad de datos por hora/día/semana/mes/año. Google Earth Engine (GEE) es un excelente lugar para obtener datos de calidad de este tipo a través de su editor de código javascript o API de python.
---

En 2022-23, la misión NISAR (el programa de radar satelital más ambicioso que se lanzará hasta el momento) generará 85 TB de datos cada día. A finales del 2021 se lanzó con éxito el telescopio espacial James Webb y debe ser difícil cuantificar la cantidad de información que enviará a la tierra en cualquier unidad de tiempo.

Por otro lado se encuentran las ciencias de la tierra, oceanográficas, ambientales, biológicas, que de una forma u otra están reconfigurando la forma en que producen conocimiento. La teledetección y los sensores remotos han impulsado esta revolución que apenas está comenzando con proyectos extremadamente ambiciosos en distintos ámbitos científicos o multidisciplinarios.

> Google Earth Engine (GEE) es un salvavidas para los investigadores al evitar la descarga de archivos pesados y que puede ralentizar su objetivo principal: el conocimiento. Ofrece datos de calidad y al alcance de todos sus usuarios. 

##### NASA, ESA, NOAA: un paraíso de open data  

Me emociona el sólo ver esas siglas y saber que puedo encontrar datos por parte de estas reconocidas y respetadas organizaciones con simplemente una cuenta de google. 

Empecemos con la NASA la cual no necesita ningún tipo presentación. Son muchos los recursos que ofrece la Administración Aeronáutica Espacial norteamericana tanto en sus plataformas como en el mismo GEE. Aqua, Terra, Aura, Landsat, SMAP, son sólo algunos nombres de su poderosa "flota" de satélites especializados en diferentes campos. Cada uno cuenta con sensores específicos que lo hacen único.

No más atrás y a la altura de las circunstancias se encuentra la Agencia Espacial Europea (ESA) con su programa Copernicus y sus elegantes satélites Sentinel. A título personal tengo una debilidad especial por este programa ya que fue el que me introdujo a todo este apasionante mundo. 

Con Copernicus viví la tediosa tarea de descargar datos e imágenes muchas veces pobres en su resolución por la cantidad de nubes, pero de igual forma ha sido reconfortante observar el avance de cómo ha evolucionado positivamente la accesibilidad a sus distintos componentes.

Para terminar con este tridente (aunque hay muchos recursos más en GEE) están los conjuntos de datos proporcionados por la Oficina Nacional Oceánica y Atmosférica de Estados Unidos (NOAA). Lo que ellos hacen es agrupar información captada por satélites, boyas y embarcaciones para ajustarlos y brindarle un producto de calidad al usuario. 


### 2 de mis favoritos: Sea Surface Temperature (SST) y Ocean Colors

NOAA aglutina información de distintas fuentes, entre ellas sobresale la temperatura superficial del mar (SST), la cual he podido aplicar de forma exitosa en diversos proyectos. Con la SST se pueden derivar estudios interesantes en cobertura coralina, blooms tóxicos algales o muerte masiva de especies marinas. [Un ejemplo de SST.](https://github.com/grammaloreto/SeaSurfaceTemperature-SST-).

Ocean Color hace referencia a las concentraciones de clorofila-a (fitoplancton) que está presente en los cuerpos de agua. Entre los sensores más conocidos tenemos a MODIS del satélite AQUA de la NASA o también OLCI de Sentinel-3 de ESA. [Un ejemplo con MODIS. ](https://github.com/grammaloreto/EarthEngine/tree/main/MODIS_Aqua_chlor_a)
[Un ejemplo con OLCI.](https://github.com/grammaloreto/EarthEngine/tree/main/Sentinel3)

Si estas interesado te recomiendo visitar, aprender e investigar con GEE. Mi repositorio completo lo dejo [aquí.](https://github.com/grammaloreto/EarthEngine)





