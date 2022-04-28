---
title: Trabajando datos de Migración Colombia con fines turísticos
date: "2022-01-30T22:12:03.284Z"
description: Esta institución aporta datos de ingreso-salida de extranjeros, ciudadanos nacionales, los medios por los cuales ingresan, la ciudad de pernoctación entre otras. En base a estas variables proporcionadas cada mes, es posible analizar y sacar conclusiones valiosas para el turismo que ha sido tan golpeado durante la pandemia. 
---

### 2020, un año atípico... pero con datos de los que se puede aprender mucho

No es común y difícilmente se repetirán los datos turísticos (ingresos/salidas de visitantes) en los meses más críticos de la pandemia. Al ser un evento espontáneo y nunca experimentado en épocas modernas, solo había opción de tomar medidas drásticas que con el tiempo han ido amoldándose más a una realidad que continua complicada en muchos aspectos.

>Una de las cosas que nos ha dejado esta difícil coyuntura son las cifras y los datos que de por sí tienen un valor incalculable. 

Poniéndonos un poco más técnicos, al realizar diferentes pruebas llama la atención la reproducibilidad y confiabilidad de los datos en el momento más álgido de la pandemia. Por ejemplo, realizando pruebas de correlación de Pearson entre las variables turísticas estudiadas, se observa un mayor grado de intensidad en 2020 a comparación de otros años recientes.

[Acá puedes ver los coeficientes de correlación completos](https://github.com/grammaloreto/Foreign-Tourism-Colombia-2018-2021/blob/main/correlations.ipynb)

Estas relaciones son importantes para evaluar que tan dependientes o independientes pueden ser las variables y así poder realizar otras pruebas predictivas o que brinden insights más valiosos.  

### Modelo de Regresión para predecir el número de turistas de Sol y Playa a partir del total de turistas extranjeros que entran al país

El modelo de Regresión Lineal se entrenó con datos que van desde el año 2017 al 2021. El objetivo: predecir el número de turistas extranjeros que viajan exclusivamente a visitar las principales ciudades y playas del Caribe colombiano (variable dependiente) a partir del número total de extranjeros que pueden ingresar al país (variable independiente). 

La confiabilidad del modelo es bastante alta y las predicciones son bastante congruentes con los datos reales. [El modelo completo en este notebook.](https://github.com/grammaloreto/Foreign-Tourism-Colombia-2018-2021/blob/main/Linear%20model%20to%20predict%20the%20number%20of%20Sun%26beach%20visitors%20.ipynb)

### Otros insights...

El año 2018 ha sido el mejor en cuanto a recepción de turistas extranjeros, siendo el mes de diciembre el pico máximo con 309.737 visitantes. Los meses de febrero y marzo de ese mismo año fueron también excepcionales con un total de 304.751 y 306.250 visitas respectivamente. 

Los años 2017 y 2019 no fueron tan exitosos como el 2018, sin embargo no se puede desconocer que presentaron números de turistas extranjeros alentadores (4.880.536 y 5.063.308 respectivamente)

El año 2020 iniciaba a buen ritmo pero como consecuencia de las primeras medidas “anti-covid” caracterizadas por los cierres de fronteras y la puesta en tierra de muchos aviones, hicieron que las proyecciones se vinieran a pique. Migración Colombia reportó en abril del 2020 la entrada de 6 turistas extranjeros, 1 para el mes de mayo, 16 en junio como en agosto y 7 para julio. Sólo hasta septiembre de ese año se produjo un incremento de 2.901 turistas extranjeros ingresando nuevamente al país. 

Vale la pena destacar a países como Estados Unidos y del Mercosur (Argentina-Brasil) como los principales en dinamizar el sector turístico en los últimos años. 

[Repositorio completo de GitHub.](https://github.com/grammaloreto/Foreign-Tourism-Colombia-2018-2021)




 
