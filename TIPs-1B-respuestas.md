<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo B --&gt; Primer Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>Se pueden realizar consultas para buscar registros duplicados en una tabla en SQL utilizando la cláusula GROUP BY y la función COUNT. Por ejemplo: 
SELECT campo
COUNT(campo) 
FROM tabla 
GROUP BY campo 
HAVING COUNT(campo) &gt; 1; </p>
<h3>2)  Respuesta:</h3>
<p>Lista: Mutable, velocidad inferior y utilización de corchetes.

Tupla: Inmutable, velocidad superior y utilización de paréntesis </p>
<h3>3)  Respuesta:</h3>
<p>Las VARIABLES GLOBALES son las declaradas fuera de una función. Todas las funciones del código pueden acceder a dicha variables. En cambio, las VARIABLES LOCALES son aquellas creadas dentro de las funciones. Intentar acceder a ellas fuera de la función devolverá una falla del sistema. </p>
<h3>4)  Respuesta:</h3>
<p>Pueden implementarse 3 tipos de filtros:</p>
<p>Filtros a nivel visualización: Filtra tanto datos como medidas calculadas, limitando la cantidad de información que puede verse en una visualización determinada.</p>
<p>Filtros a nivel página: Filtra la info en todas las visualizaciones de una página específica del reporte.</p>
<p>Filtros a nivel reporte: se aplican a todas las páginas y visualizaciones en simultáneo.</p>
<h3>5)  Respuesta:</h3>
<p>La probabilidad condicional es la probabilidad de que un evento ocurra dado que otro evento ya ha ocurrido. La probabilidad condicional se calcula dividiendo la probabilidad del evento conjunto por la probabilidad del evento condicionante.</p>
<h3>6)  Respuesta:</h3>
<p>a) 8 casos favorables de 20 posibles. RTA 0.4</p>
<p>b)La probabilidad de que al sacar 2 papeles al menos tenga un coche menos la probabilidad de que al sacar 2 papeles las dos sean blancas. Por lo tanto:
= 1 - P(2 Blancas)
= 1 - (12/20)*(12/20)
= 1 - 0.36
= 0.64</p>
<p>c) Tenemos la probabilidad de que al sacar 3 papeles al menos una tenga un coche menos la probabilidad de que al sacar 3 todas sean blancas. Por lo tanto:
= 1 - P(3 Blancas)
= 1 - (12/20)*(12/20)*(12/20)
= 0.784</p>
