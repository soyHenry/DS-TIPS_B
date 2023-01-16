
# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1)Describa y explique los diferentes tipos de JOINS para SQL.**


__Respuesta Esperada__:  

_- INNER JOIN: Devuelve todas las filas cuando hay al menos una coincidencia en ambas tablas._  
_- LEFT JOIN: Devuelve todas las filas de la tabla IZQUIERDA y las filas coincidentes de la tabla de la derecha._  
_- RIGHT JOIN: Devuelve todas las filas de la tabla DERECHA y las filas coincidentes de la tabla de la izquierda._  
_- OUTER JOIN: Devuelve todas las filas de las dos tablas. También conocida como FULL OUTER JOIN.__
  
<br>
  
### **2) Se sacan dos bolas de una urna que se compone de una bola blanca, otra roja, otra verde y otra negra. Describa el espacio muestral cuando:**  

**a) La primera bola se devuelve a la urna antes de sacar la segunda.**  
**b) La primera bola no se devuelve.**



__Respuesta Esperada__:   

_a) E = {BB,BR,BV,BN,RB,RR,RV,RN,VB,VR,VV,VN,NB,NR,NV,NN}_  

_b) E={BR,BV,BN,RB,RV,RN,VB,VR,VN,NB,NR,NV._
                          

<br>
  
### **3) ¿Cuál es la principal diferencia entre una métrica y un KPI?**


__Respuesta Esperada__:   _Los KPI difieren de las métricas en la forma en la que se utilizan. Mientras que una métrica mide un valor crudo sobre un proceso, un KPI está asociado directamente a un objetivo marcado por la empresa y permite evaluar si las estrategias seguidas para conseguirlo están funcionando._

<br>

  
### **4) ¿Qué son las formas normales en bases de datos?**
 
__Respuesta Esperada:__:  
_Son una serie de normas que se aplican a las tablas de datos para cumplir con la propiedad deseable de no redundancia. Son 5 formas normales y en general, se considera que una base de datos está correctamente normalizada si llega por lo menos a la tercera forma normal (3F)_


## **5) Ejercicio practico python: 'Mover los ceros'**  

Dada una cadena de caracteres en minúscula, crear una función que sólo devuelva las vocales del string

`Input`: onomatopeya  
`Output`: ooaoea

  
__Respuesta Esperada__:

```python
def filtrar_vocales(string):  
    for i in string:  
        vocales =['a','e','i','o','u']
        if i in vocales:  
            print(i, end = '')  

filtrar_vocales('onomatopeya');
 ```
