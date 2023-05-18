<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo B --&gt; Segundo Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>Se pueden realizar consultas para buscar registros duplicados en una tabla en SQL utilizando la cláusula GROUP BY y la función COUNT. Por ejemplo: 
SELECT campo
COUNT(campo) 
FROM tabla 
GROUP BY campo 
HAVING COUNT(campo) &gt; 1; </p>
<h3>2)  Respuesta:</h3>
<p>El 'index' es el "índice" de DataFrame, se aplica normalmente a la referencia de un dato en una estructura según su posición, para poder referenciar cada fila. Se puede acceder a través del atributo .index de pandas, que devuelve la representación de él. Puede haber más de un índice en el DataFrame, estas estructuras poseen MultiIndex, que es un índice funcionando a varios niveles de jerarquía, donde múltiples columnas de índice refieren a una fila. Permiten análisis de datos multidimensionales. </p>
<h3>3)  Respuesta:</h3>
<p>La recursividad en Python es una técnica en la que una función se llama a sí misma repetidamente hasta alcanzar un caso base. La recursividad puede ser muy útil en situaciones en las que una solución se puede dividir en subproblemas más pequeños. </p>
<h3>4)  Respuesta:</h3>
<p>Columna Calculada:</p>
<p>Se agregan a tablas existentes mediante fórmulas DAX sobre columnas existentes. Define y almacena valores en una columna nueva sin hacer query a la fuente de datos. </p>
<p>Tabla calculada:</p>
<p>Creada mediante fórmula DAX para definir todos sus valores. Puede crearse tanto en Vista Reporte como en Vista Data. </p>
<p>Medidas:</p>
<p>Se realiza a través de la query.</p>
<h3>5)  Respuesta:</h3>
<p>Media: (7+5+8+6+4+9+6+8+7+5)/10 = 6.5

Mediana: ordenando los datos: 4, 5, 5, 6, 6, 7, 7, 8, 8, 9. La mediana es el valor medio entre el quinto y sexto número, es decir, (6 + 7)/2 = 6.5

Desviación estándar: primero se calcula la varianza, que es la suma de los cuadrados de las desviaciones de cada punto de la media dividido por n-1. (7-6.5)^2 + (5-6.5)^2 + (8-6.5)^2 + (6-6.5)^2 + (4-6.5)^2 + (9-6.5)^2 + (6-6.5)^2 + (8-6.5)^2 + (7-6.5)^2 + (5-6.5)^2 = 55.5. Entonces, la desviación estándar es la raíz cuadrada de la varianza dividida por n-1: sqrt(55.5/9) = 2.20</p>

<h3>6)  Respuesta:</h3>
<p>La regresión lineal es un método estadístico que se utiliza para modelar la relación entre una variable dependiente y una o más variables independientes. La regresión lineal se utiliza para predecir el valor de la variable dependiente en función de los valores de las variables independientes. </p>
