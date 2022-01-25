---
title: Cómo descubrir nuevas medicinas con Python
date: "2022-01-24T22:40:32.169Z"
description: Los ensayos farmacológicos y gran parte del desarrrollo de nuevas medicinas se está transformando con la accesibilidad de herramientas e información al alcance de todos.  
---

El paradigma dominante en el descubrimiento de fármacos y que es inmutable con el pasar del tiempo es el concepto de diseñar ligandos (moleculas no tan grandes) para actuar sobre objetivos específicos (Targets). Pueden crearse ligandos de gran afinidad u otros mas "generalistas", estos últimos mas populares en la actualidad.

## Chembl y PubChem 

Estos son 2 de las bases de datos mas populares que se encuentran en la web con informacion de todo tipo de proteinas, enzimas u otras moleculas relacionadas a ensayos clinicos y farmacologicos. Algunas estan en fases mas avanzadas, otras son incipientes pero con gran potencial.

### Python como protagonista

No es un secreto que Python es el lenguaje de programacion de la Ciencia por excelencia. Con comandos básicos y otros no tanto se pueden extraer los datos de las moleculas con las que se va a trabajar, organizar, transformar, analizar, visualizar y modelar. 

> Es importante tener conocimiento del dominio además de leer e investigar del tema.
> Conceptos escenciales, las fases de los ensayos clinicos y otra información
> relevante no está de mas.

Existen librerias de Python que facilitan la labor. RDKit es una de ellas. Con este paquete es mas fecil manipular y modelar las distintas estructuras moleculares. Si la vas a usar sera una buena herramienta para incursionar en el campo de la quimioinformática en trabajos posteriores.

### Las reglas de Lipinski y la concentracion IC50

A la hora de refrescar conceptos relacionados al descubrimiento de medicinas estos 2 podrian estar encabezando la lista. 

En primer lugar están las relgas de Lipinski que son basicamente enunciados empiricos a cumplir por un compuesto quimico para poder ser considerado con algun tipo de actividad farmacologica. Se podria nombrar la masa molecular o el numero de atomos que aceptan enlaces o forman puentes de hidrogeno.

Por otro lado se encuentra la concentracion inhibidora que un farmaco necesita para inhibir un proceso biologico (IC50). Esta medida es fundamental a la hora de determinar la eficiencia o toxicidad de algun compuesto de interes. Existen otras concentraciones o constantes relacionadas que brindan mayor informacion cuantitativa de las moleculas. 

#### Descriptores y Machine Learning

Una vez se hayan analizado las moleculas y evaluado si son inactivas o inactivas dependiendo de las variables consideradas, podrian realizare otro tipo de procesos informaticos para conocer mejor las relaciones y similitudes entre ligandos y targets. 

Para lograr esto se llevan a cabo transformaciones de las moleculas mediante descriptores, los cuales convierten las propiedades quimicas de una molecula (como su estructura o numero de atomos) en numeros binarios (u otro tipo de representaciones) para poder modelarlas.

Al tener las moleculas representadas en datos de entrada para modelos de Machine Learning es cuestion de escoguer el modelo mas adecuado o que vaya a tener una mejor reproducibilidad. En nuestro [repositorio](https://github.com/grammaloreto/Bioactivity) se escogió Random Forest.  

##### El caso Particular de este estudio.

El target que se escogió para este repositorio fue PSMB5, una sub-unidad del complejo de proteasomas (presente en todas las celulas humanas) que tiene entre muchas otras funciones la degradacion de proteinas dañadas o que ya no son necesarias. Este complejo ha sido ampliamente estudiado para tratar canceres, Alzheimer y Parkinson.

Finalmente y como compuesto de interes entre las moleculas activas para este target se puede mencionar al Borteozomib, de gran accion citotoxica con celulas tumorales que inhiben la accion del proteasoma. Una vez se hayan obtenido buenos resultados con determinados complejos proteicos seria pertinente continuar ensayos con sustancias similares. 

Puedes ver el repositorio completo en [GitHub](https://github.com/grammaloreto/Bioactivity)
