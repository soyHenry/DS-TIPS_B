
# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1)¿Qué son los iteradores de Python? Ejemplifique.**

__Respuesta Esperada__:   _Los iteradores son objetos que contienen algunos valores contables. Ejemplo listas, tuplas, conjuntos y diccionarios._

<br>

### **2)¿Qué es una serie en pandas?**

__Respuesta Esperada__:   _Es un tipo de Arreglo similar a un array de NumPy que te permite almacenar información de diversa tipología ; sea por medio de cadenas de texto , flotantes o enteros, dtype, entre otros (a diferencia del array de NumPy que debe ser sólo de un tipo). En un nivel más sutil puedes incluso trabajar con constructores y toda una diversidad de métodos._

  <br>

### **3) ¿Cuáles son los diferentes tipos de vistas disponibles en POWER BI Desktop?**

__Respuesta Esperada__:   _Hay 3 tipos de vistas disponibles, cada una con un propósito diferente:
Vista Reporte: permite añadir páginas, visualizaciones y publicar
Vista de Data: permite realizar manejo de datos usando herramientas de Query Editor.
Vista de Modelo: permite manejar las relaciones entre las tablas de datos._


<br>


## Suponga que tiene las tablas *SALAS* y *PELICULAS* compuestas de la siguiente forma.

### SALAS                     

| `PK` | Codigo | int |
|--------|--------|:--------:|
|  | Nombre | nvarchar(100) |
| `FK1`  | Pelicula  | int |
  

### PELICULAS
  
| `PK` | Codigo | int |
|--------|:--------|:--------:|
|  | Nombre | nvarchar(100) |
|  | CalificacionEdad  | int |
  
Note que existe una relacion entre *`FK1` - Pelicula* de la tabla SALAS y *`PK`-Codigo* de la tabla PELICULAS
  
<br>

## Con dichas tablas construya las siguientes queries:
### **4) Seleccione los valores unicos de calificaciones de edad que existen.**
<br>
  
__Respuesta Esperada__:
```sql
SELECT DISTINCT CalificacionEdad 
FROM PELICULAS
```


### **5) Se ha agregado una nueva pelicula llamada "Hola, Mundo" para mayores de 8 años. Actualice la tabla correspondiente**
<br>
  
__Respuesta Esperada__:
```sql
INSERT INTO PELICULAS (Nombre, CalificacionEdad)
VALUES ("Hola, Mundo", 8)
```

  
### **6) Seleccione todas las salas, y si se proyecta alguna pelicula en la sala, selecciones tambien la informacion de la pelicula proyectada**
  
<br>
  
__Respuesta Esperada__:   

```sql
SELECT *
FROM SALAS LEFT JOIN PELICULAS
ON SALAS.Pelicula = PELICULAS.Codigo
```
<br>
  
