---
title: Análisis de sentimientos con BERT y transformadores de Hugging Face
date: "2022-01-10T23:46:37.121Z"
description: Los comentarios en redes y sitios web dejaron de ser subjetivos, son buenos, malos o podrian clasificarse en un termino medio (pero mas cercanos al lado positivo o negativo). Mediante los transformadores de procesamiento de lenguaje natural (NLP) se les puede dar un valor cuantitativo y tener una idea mas clara de la percepcion de un cliente o consumidor.
---

Los números tienen la verdad! sin rodeos y sin darle tantas vueltas a cierto producto, lugar, incluso persona, hoy en dia es posible determinar con certeza cual es la opinion de alguien a partir de algun comentario, review, post, palabra.

Mediante las distintas herramientas de Procesamiento de Lenguaje Natural (NLP) no hay limitantes de idioma, modismos, semantica, sintaxis o de algun otro tipo de expresion linguistica.

##### 2 Herramientas muy poderosas para todo tipo de lenguajes

Hugging Face y Bert son 2 de las muchas tecnologias pioneras y que engrandecen a este dominio. El primero es una compañia con distintas librerias aplicadas a varios campos de NLP. Ofrecen modelos basados en transformadores a traves de PyTorch y Tensorflow.

Por otro lado tenemos a BERT (Bidirectional Encoder Representations from Transformers), propiedad de Google y usado en el complejo entramado de redes neuranales para procesar e interpretar todo tipo de lenguajes en dicho motor. Ambos modelos son extremadamente efectivos por el poderoso entrenamiento brindado con todo tipo de datos.

##### El poder de las palabras

Muchas veces todos hemos tomado desiciones en base a algun comentario o calificaicon hecha en portales o redes sociales. Ahora serà todo mas facil, un texto largo brindando cierta opinion puede ser traducido a un numero de acuerdo a las palabras que lo conforman. 

En este caso se analisan comentarios de 8 de las playas mas turisticas de Colombia. Bien se sabe que es uno de los principales atractivos del país y como parte de la reactivacion del turismo y de la exigencia cada vez mayor de los visitantes es primordial tener presente la percepcion que se llevan.

#### Web Scraping para extraer los comentarios

Sin comentarios no se puede hacer nada. Es primordial tener presente distintans tecnicas ya que aveces es necesario tomar gran cantidad de datos. Para lograr el cometido es necesario saber de web scraping y de tratar el contenido de la mejor forma.

En este caso se usó Beatiful Soup, una biblioteca de Python ampliamente usada y conocida, a la par de Selenium que es otro modulo con propiedades muy similares. En este [repositorio](https://github.com/grammaloreto/Web-Scraping) puedes conocer algunas tecnicas de web scraping.

#### El estudio:

8 playas del Caribe colombiano fueron seleccionadas para hacerles un Análisis de Sentimientos. 20 comentarios (10 español, 10 inglés) fueron extraídos por playa y asi procesarlos con tranformadores para obtener una calificacion de 1-5 en base a las palabras usadas.

Los comentarios en ingles eran de todo tipo de visitantes extranjeros no latinoamericanos mientras que los tomandos en castellano eran en su mayoria de turistas nacionales, con algunas excepciones. Los transformadores y BERT no tienen limitantes de idioma por lo que podrian tomarse cualquier tipo de comentario.


#### Que opinan los visitantes nacionales y extranjeros de la playas colombianas

Juntando todos los comentarios se tiene que en promedio los turistas (nacionales e internacionales) le dan a las playas del caribe colombiano una calificación de 3.49.

Las playas mejor calificadas son las del Cabo de la Vela (Guajira) con una calificación global de 4.5, seguida por Playa San Luis (San Andres y Providencia) y Playa Cristal(Magdalena) con un puntaje de 4.0 y 3.95 respectivamente.

A Playa Blanca de Barú no le fue muy bien con los comentarios nacionales y extranjeros. Con un promedio de 2.75 fue la que peor percepción tiene por parte de sus visitantes. Esta baja calificación se debe principalmente al excesivo ”acoso” por parte de los vendedores ambulantes, la baja calidad de los servicios como de la higiene de la playa y a la cantidad de gente presente (desorganizacion).

Otra de las Playas que estuvo entre los valores mas bajos fue la de Johnny Cay en San Andres y Providencia. Paradojicamente esta playa es de las unicas que cuentan con el reconocimiento de Bandera Azul en el país. Las principales quejas y que le bajan notoriamente el atractivo a este lugar son respecto a los lancheros, el muelle y cómo no hay una organización para llegar a este lugar.

Si quieres conocer mas de este estudio o de como trabajar NLP con transformadores puedes ir a este [repositorio de Github](https://github.com/grammaloreto/SentimentAnalysis) o puedes revisar directamente este [mapa](https://grammaloreto.github.io/MapSentimentAnalysis/) con las calificaciones.


