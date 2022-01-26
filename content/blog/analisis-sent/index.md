---
title: Análisis de sentimientos con BERT y transformadores de Hugging Face
date: "2022-01-10T23:46:37.121Z"
description: Los comentarios en redes y sitios web dejaron de ser subjetivos. Son buenos, malos o podrían clasificarse en un término medio (pero más cercanos al lado positivo o negativo). Mediante los transformadores de procesamiento de lenguaje natural (NLP) se les puede dar un valor cuantitativo y tener una idea más clara de la percepción de un cliente o consumidor.
---

Los números tienen la verdad! sin rodeos y sin darle tantas vueltas a cierto producto, lugar, incluso persona, hoy en día es posible determinar con certeza absoluta cual es la opinión de alguien a partir de algún comentario, reseña, post, palabra.

Mediante las distintas herramientas de Procesamiento de Lenguaje Natural (NLP) no hay limitantes de idioma, modismos, semántica, sintaxis o de otro tipo de expresión linguística.

##### 2 Herramientas muy poderosas para todo tipo de lenguajes

Hugging Face y Bert son 2 de las muchas tecnologías pioneras y que engrandecen a este dominio. El primero es una compañía con distintas librerías aplicadas a varios campos de NLP. Ofrecen modelos basados en transformadores a través de PyTorch y Tensorflow.

Por otro lado, tenemos a BERT (Bidirectional Encoder Representations from Transformers), propiedad de Google y usado en el complejo entramado de redes neuranales para procesar e interpretar todo tipo de lenguajes en dicho motor. Ambos modelos son extremadamente efectivos por el poderoso entrenamiento que han tenido año tras año con gran cantidad de datos.

##### El poder de las palabras

Muchas veces todos hemos tomado decisiones en base a algún comentario o calificación hecha a traves de portales o redes sociales. Ahora será todo más fácil, un texto extenso brindando cierta opinión puede ser traducido a un número de acuerdo con las palabras que lo conforman. 

En nuestro caso para aplicar herramientas de NLP se analizan comentarios de las playas más turísticas de Colombia. Bien se sabe que estos lugares son de los principales atractivos del país y como parte de la reactivación del turismo es primordial tener presente la percepción que se llevan sus visitantes.

#### Web Scraping para extraer comentarios

Sin la materia prima no se puede hacer nada, es por eso primordial tener presente distintas técnicas para poder tomar gran cantidad de datos (comentarios). Para lograr el cometido es necesario saber de alguna librería o herramienta de web scraping.

En este caso se usó Beautiful Soup, una biblioteca de Python ampliamente usada y conocida, a la par de Selenium que es otro de los módulos con propiedades similares. En este [repositorio](https://github.com/grammaloreto/Web-Scraping) puedes conocer algunas técnicas de web scraping.

#### El estudio:

8 playas del Caribe colombiano fueron seleccionadas para hacerles un Análisis de Sentimientos. 20 comentarios (10 español, 10 inglés) fueron extraídos por playa y así poder procesarlos con transformadores para obtener una calificación de 1-5 en base a las palabras usadas.

Los comentarios en inglés eran de todo tipo de visitantes extranjeros no latinoamericanos, mientras que las reseñas en castellano eran en su mayoría de turistas nacionales, con algunas excepciones. Cabe recordar que los transformadores y BERT no tienen limitantes de idioma pero la división se hizo mas que todo para diferenciar percepciones.


#### Qué opinan los visitantes nacionales y extranjeros de las playas colombianas?

Juntando todos los comentarios se tiene que en promedio los turistas (nacionales e internacionales) le dan a las playas del Caribe colombiano una calificación de 3.49.

Las playas mejor calificadas son las del Cabo de la Vela (Guajira) con una calificación global de 4.5, seguida por Playa San Luis (San Andrés y Providencia) y Playa Cristal (Magdalena) con un puntaje de 4.0 y 3.95 respectivamente.

A Playa Blanca de Barú no le fue muy bien con los comentarios nacionales y extranjeros. Con un promedio de 2.75 fue la que peor percepción tiene por parte de sus visitantes. Esta baja calificación se debe principalmente al excesivo "acoso" por parte de los vendedores informales, la baja calidad de los servicios como de la higiene de la playa y a la cantidad de gente presente (desorganización).

Otra de las Playas que estuvo entre los valores más bajos fue la de Johnny Cay en San Andrés y Providencia. Paradójicamente esta playa es de las únicas que cuentan con el reconocimiento de Bandera Azul en el país. Las principales quejas y que le bajan notoriamente el atractivo a este lugar son respecto a los lancheros, el muelle y cómo no hay una organización para llegar a este lugar.

Si quieres conocer más de este post o de como trabajar NLP con transformadores puedes ir a este [repositorio de GitHub](https://github.com/grammaloreto/SentimentAnalysis) o puedes revisar directamente el [mapa](https://grammaloreto.github.io/MapSentimentAnalysis/) con las calificaciones.


