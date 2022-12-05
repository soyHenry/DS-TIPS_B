
# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1) ¿Qué es la normalización de la base de datos?**

__Respuesta Esperada__:   _Proceso de análisis de las relaciones de los datos basado en sus dependencias funcionales y claves primarias para conseguir las siguientes propiedades deseables:_

  
  _1)Minimizar la redundancia_

  _2) Minimizar las anomalías de inserción, borrado y actualización_

_Si los esquemas de relación no cumplen las propiedades, se descomponen en esquemas de relación más pequeños que puedan cumplir con las propiedades deseables (Formas Normales)._
  
<br>
  
### **2)¿Qué es una subconsulta? Explique de manera breve su sintaxis.**

__Respuesta Esperada__:   _Una subconsulta es una consulta hecha sobre otra consulta._

  
  SELECT <column_name>
  
  FROM <table_name> 
  
  WHERE <column_name> IN/NOT IN  (subconsulta).
  
                           

<br>
  
### **3) ¿Puede citar algunos ejemplos en los que un falso positivo sea más importante que un falso negativo?**


__Respuesta Esperada__:   _En medicina podría significar la toma de medidas de tratamiento demasiado apresuradas cómo recibir medicamentos que no necesitan, a veces con efectos secundarios peligrosos; o conducir a procedimientos innecesarios, en ocasiones permanentes. 
Por ejemplo, una mujer en edad fértil que recibe un falso positivo por cáncer cervicouterino, podría someterse a una histerectomía innecesaria. Como resultado, perdería su capacidad de tener hijos._

<br>
  <br>
  



## Ejercicio practico python: 'Mover los ceros'
Dada una lista de numeros, escriba una funcion que mueva todos los ceros al final
de la lista, manteniendo el orden relativo de los numeros que no son 0.

`Input`: [0, 1, 0, 3, 12]
  
`Output`: [1, 3, 12, 0, 0]

  
__Respuesta Esperada__:

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
