---
title: Cómo descubrir nuevas medicinas con Python
date: "2022-02-02T22:40:32.169Z"
description: Los ensayos farmacológicos y gran parte del desarrollo de nuevas medicinas se está transformando con la accesibilidad de herramientas e información al alcance de todos.  
---

El paradigma dominante en el descubrimiento de fármacos y que es inmutable con el pasar del tiempo es el concepto de diseñar ligandos (moléculas no tan grandes) para actuar sobre objetivos específicos (Targets). Pueden crearse ligandos de gran afinidad u otros más "generalistas", estos últimos con mayor popularidad en la actualidad.

### ChEMBL y PubChem 

Estas son 2 de las bases de datos más populares que se encuentran en la web, con información de todo tipo de proteínas, enzimas u otras moléculas relacionadas a ensayos clínicos y farmacológicos. Algunas están en fases más avanzadas, otras son incipientes pero con gran potencial.

#### Python como protagonista

No es un secreto que Python es el lenguaje de programación de la Ciencia por excelencia. Con comandos básicos y otros no tanto se pueden extraer datos de las moléculas con las que se va a trabajar, analizar, visualizar y modelar. [Código ejemplo para extraer datos de ChEMBL.](https://github.com/grammaloreto/Bioactivity/blob/main/dataCollection_ChEMBL/PSMB5.ipynb)

> Es importante tener conocimiento del dominio además de leer e investigar del tema.
> Conceptos esenciales, las fases de los ensayos clínicos y otra información
> relevante no está de mas.

Existen librerías de Python que facilitan la labor. RDKit es una de ellas. Con este paquete es más fácil manipular y modelar las distintas estructuras moleculares. Si la vas a usar será una buena herramienta para incursionar en el campo de la quimioinformática.

#### Las reglas de Lipinski y la concentración IC50

A la hora de refrescar conceptos relacionados al descubrimiento de medicinas estos 2 podrían encabezar la lista. 

En primer lugar tenemos las reglas de Lipinski, que son básicamente enunciados empíricos a cumplir por un compuesto químico para poder ser considerado con algún tipo de actividad farmacológica. Se podría mencionar la masa molecular o el número de átomos que aceptan enlaces o forman puentes de hidrogeno.

Por otro lado, se encuentra la concentración que un fármaco necesita para inhibir un proceso biológico (IC50). Esta medida es fundamental a la hora de determinar la eficiencia o toxicidad de algún compuesto de interés. Existen otras concentraciones o constantes relacionadas que brindan mayor información cuantitativa de las moléculas usadas en ensayos. 

#### Descriptores y Machine Learning

Una vez se hayan analizado las moléculas y evaluado si son activas o inactivas dependiendo de las variables consideradas, podrían realizare otro tipo de procesos informáticos para conocer mejor las relaciones y similitudes entre ligandos y targets. 

Para lograrlo se llevan a cabo transformaciones mediante descriptores, los cuales convierten las propiedades químicas de una molécula (como su estructura o número de átomos) en números binarios para así poderlas modelar.

Al tener las moléculas representadas en datos de entrada para modelos de Machine Learning, lo siguiente sería escoger el modelo más adecuado o que vaya a tener una mejor reproducibilidad. En nuestro [caso](https://github.com/grammaloreto/Bioactivity/blob/main/RandomForest/PSMB5_model.ipynb) se escogió Random Forest.  

#### El caso Particular de este estudio

El target escogido fue PSMB5, una sub-unidad del complejo de proteasomas (presente en todas las células humanas) que tiene entre muchas otras funciones la degradación de proteínas dañadas o que ya no son necesarias. Este complejo ha sido ampliamente estudiado para tratar cáncer, Alzheimer y Parkinson.

Finalmente y como compuesto de interés entre las moléculas activas para este target concreto se puede mencionar la Borteozomib, de gran acción citotóxica con células tumorales que inhiben la acción del proteasoma. Una vez se hayan obtenido buenos resultados con determinados complejos proteicos sería pertinente continuar ensayos con sustancias similares. 

Puedes ver el repositorio completo en [GitHub.](https://github.com/grammaloreto/Bioactivity)
