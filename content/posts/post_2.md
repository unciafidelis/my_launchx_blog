---
title: "MarkDown Sintaxis básica"
date: 2022-04-22
description: 'El arte de escribir documentación de proyectos en github'
---

# MarkDown Sintaxis básica - Tablas y encabezados 

### El arte oculto de escribir documentación de proyectos en github

Para enseñarme a utilizar Markdown me estoy forzando a replicar cada aspecto de la página oficial https://www.markdownguide.org/basic-syntax/
pero mostrando el código (wink*), claro esto no será una tarea fácil, pero me concentraré en cada tema para que sea más digerible así que comencemos 
con la primer tabla, la tabla de headings.

Para realizar esta tabla pues primero requiero de saber como hacer una tabla cierto? así que hice esta busqueda en google:

how to make a table in Markdown (Que!? creiste que no sabia inglés?)

y me pasó directo a la respuesta, la página https://hackmd.io/s/how-to-create-table:

con el ejemplo:

html = markdown(s, extensions=['tables'])

|Name |Quantity
|:----:|:----:
|Apple|3       
|Egg  |12      

que en código sería:

```markdown
|Name|Quantity
|:----:|:----:
|Apple|3       
|Egg  |12      
```
Por cierto para que se vea el código solo tienen que utilizar lo siguiente:


\```markdown(aqui tambien puedes poner javascript por ejemplo y así le dará formato de javascript)
   aqui va el código de markdown
\```

Las triples backticks(Sí, así se llaman... ok comilla al revés para los compas) marcan el principio y el final del código, mientras que markdown en este caso
representa un lenguaje. El uso de la \ fue para omitir el formato de markdown en orden de poder colocar las backticks y 
que se vean todas bonitas ahí, si no lo hacia solo verían el "aqui va el código de markdown" en el apartado.

Bueno ahora que ya sabemos hacer una tabla solo hay que vaciar los datos de como hacer un encabezado y su resultado:

|Markdown|HTML| Rendered Output   
|:----:|:----:|:----:
|# Heading     |Etiqueta H1|<h1>Heading</h1>  	
|## Heading    |Etiqueta H2|<h2>Heading</h2>	
|### Heading   |Etiqueta H3|<h3>Heading</h3>	
|#### Heading  |Etiqueta H4|<h4>Heading</h4>	
|##### Heading |Etiqueta H5|<h5>Heading</h5>	
|###### Heading|Etiqueta H6|<h6>Heading</h6>	


La tabla es ligeramente diferente a la original pero para mi se entiende mejor je.
Ahora el código:

```markdown
|Markdown|HTML| Rendered Output   
|:----:|:----:|:----:
|# Heading     |Etiqueta H1|<h1>Heading</h1>  	
|## Heading    |Etiqueta H2|<h2>Heading</h2>	
|### Heading   |Etiqueta H3|<h3>Heading</h3>	
|#### Heading  |Etiqueta H4|<h4>Heading</h4>	
|##### Heading |Etiqueta H5|<h5>Heading</h5>	
|###### Heading|Etiqueta H6|<h6>Heading</h6>	
```
Como podemos ver el simbolo numeral (el gatito pues) agrega un nivel al tamaño de la letra haciendola mas pequeña con cada numeral agregado, 
que como en la sintaxis de HTML, a medida que incrementa el número de H (<H(número de h)>) disminuye su tamaño.

Observa que hay un espacio entre el numeral y el nombre del encabezado, si lo omites pasará esto:

#Esto no tiene espacio pero si un numeral

al contrario de:

# Esto SI tiene un espacio y un numeral

hay otra manera de hacer encabezados pero la neta nadie en su sano juicio la utilizaría... así que para que todos mantengamos cordura y practicidad
quedémonos con este sencillo método.

Ahora ya sabes hacer tablas y encabezados en Markdown! WHAT!?

Edit: Al parecer tuve un problema con las tablas y el como se desplegaron en mi blog, así que hice una pequeña búsqueda en la
documentación de HUGO en el apartado de tables a ver que pasa y pues hice la modificación para centrar los elementos
dentro de las tablas, haré el commit y veremos como se ve en el blog.

DIGO QUE JALA!
