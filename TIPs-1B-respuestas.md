<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo B --&gt; Primer Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>Una subconsulta es una consulta que se ejecuta dentro de otra consulta, mientras que una unión combina los resultados de dos o más consultas en una sola tabla. </p>
<h3>2)  Respuesta:</h3>
<p>NumPy es un paquete de módulos muy popular en Python, que permite realizar operaciones matemáticas y algebraicas muy fácil y eficientemente, gracias a su estructura de datos, llamada Array (o arreglo) que, al tener sólo un tipo de dato (a diferencia de las listas que pueden tener al mismo tiempo strings, floats, e incluso diccionarios o listas) permite trabajar mucho más eficientemente y aparte permite almacenar datos en varias dimensiones. </p>
<h3>3)  Respuesta:</h3>
<p>El 'index' es el "índice" de DataFrame, se aplica normalmente a la referencia de un dato en una estructura según su posición, para poder referenciar cada fila. Se puede acceder a través del atributo .index de pandas, que devuelve su representación. Puede haber más de un índice en el DataFrame, estas estructuras poseen MultiIndex, que es un índice funcionando a varios niveles de jerarquía, donde múltiples columnas de índice refieren a una fila. Permiten análisis de datos multidimensionales. </p>
<h3>4)  Respuesta:</h3>
<p>Hay 3 tipos de vistas disponibles, cada una con un propósito diferente:</p>
<p>Vista Reporte: permite añadir páginas, visualizaciones y publicar</p>
<p>Vista de Data: permite realizar manejo de datos usando herramientas de Query Editor</p>
<p>Vista de Modelo: permite manejar las relaciones entre las tablas de datos</p>
<h3>5)  Respuesta:</h3>
<p>La probabilidad condicional es la probabilidad de que un evento ocurra dado que otro evento ya ha ocurrido. La probabilidad condicional se calcula dividiendo la probabilidad del evento conjunto por la probabilidad del evento condicionante.</p>

<h3>6)  Respuesta:</h3>
<p>a) E = {BB,BR,BV,BN,RB,RR,RV,RN,VB,VR,VV,VN,NB,NR,NV,NN}</p>
<p>b) E={BR,BV,BN,RB,RV,RN,VB,VR,VN,NB,NR,NV}</p>

## Ejercicio practico python: 'Mover los ceros'
Dada una lista de numeros, escriba una funcion que mueva todos los ceros al final
de la lista, manteniendo el orden relativo de los numeros que no son 0.

`Input`: [0, 1, 0, 3, 12]
  
`Output`: [1, 3, 12, 0, 0]

  
__Solucion propuesta__:

```python
lista1 = [0,1,0,3,12]
lista2 = [1,7,0,0,8,0,10,12,0,4]

def mueve_0s(nums):
    for i in nums:
        if 0 in nums:
            nums.remove(0)
            nums.append(0)
    return nums

mueve_0s(lista1)
mueve_0s(lista2)
 ```

