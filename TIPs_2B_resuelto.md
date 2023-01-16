
# Bienvenidos a las TIP's. 
Recuerda que esto es una herramienta para practicar como seria una entrevista real! Pero en un ambiente seguro :blush:<br>
Bajo ningun punto de vista queremos su compañer@ pase un mal momento! Simplemente guialo a traves de las preguntas<br>
<sub>No le des las respuestas facilmente, pero sueltale pistas si l@ ves un poco perdido@ :wink:

<br>
  
### **1)¿Qué es la complejidad algorítmica? ¿Con qué símbolo o letra se representa la notación de la cota superior?**

__Respuesta Esperada__:   
_La complejidad algorítmica representa la cantidad de recursos (temporales) que necesita un algoritmo para resolver un problema y por tanto permite determinar la eficiencia de dicho algoritmo.  
En términos de notación, en la complejidad algorítmica se suele emplear una contracción que exprese de igual manera la naturaleza del algoritmo en cuestión, es decir, para una complejidad polinomial Θ(5n² + 8n + 3), se sintetizará la expresión tomando solo la literal con el mayor grado relativo, quedando expresado como Θ(n²). Esta notación se conoce como Orden de Complejidad algorítmica._

<br>

### **2) Se lanzan dos dados al aire y se anota la suma de puntos obtenidos. Se pide:**  
**a) La probabilidad de que salga 7.**  
    
**b.  La probabilidad de que el número obtenido sea par.**   
<br>

__Respuesta Esperada__:   
_a)_ 
  _i. Casos Favorables: $$6 \longrightarrow (1+6),(2+5),(3+4)...$$_   
  _ii.Casos Posibles: $${6^2}  = 36$$_  
  _iii.Probabilidad: $$\dfrac{Casos Favorables}{Casos Posibles} = \dfrac{6}{36} = 0.1666...$$._

_b)_  
  _i. Casos Favorables: 18_  
  _ii. Casos posibles: 36_  
  _iii. Probabilidad: $$\dfrac{Casos Favorables}{Casos Posibles} = \dfrac{18}{36}= 0.5$$_

<br>

### **3) Nombre los diferentes objetos de una base de datos (pista: 6 son permanentes y 1 temporal)**  
<br>

__Respuesta Esperada__:   
_Permanentes: Table, Views, Procedures, Functions (definidas por el usuario), Triggers, Indexes.  
Temporales: Cursors._


<br>

### **4) ¿Qué librerías de visualización para Python conocen? ¿Y para graficar mapas geográficos? ¿Y para realizar Dashboards?**  
<br>

__Respuesta Esperada__:  

_Hay muchas. Entre las más utilizadas para realizar visualizaciones varias está matplotlib (de muy bajo nivel), seaborn (construida sobre matplotlib), plotly (muy completa y de alto nivel, permite simplificar mucho la sintaxis para realizar gráficos interactivos pero es computacionalmente más costosa), plotnine (muy similar a ggplot2 muy usado en el lenguaje R), Gleam (muy similar a Shiny en el lenguaje R), missingno (muy útil para lidiar con datos faltantes), leather (permite generar gráficos simples pero en formato SVG muy escalables a cualquier resolución), Bokeh (permite gráficos interactivos) y Altair (permite gráficos interactivos muy llamativos). Para mapas, pueden utilizar Plotly, Bokeh, Altair, la librería Folium permite crear mapas interactivos muy personalizables y computacionalmente más baratos que plotly, también está la librería Geoplotlib. Para los dashboards, se puede utilizar Bokeh, Dash o Streamlit._
<br>


## Suponga que tiene las tablas *Ciudad* y *Pais* compuestas de la siguiente forma.  

### Ciudad                 

| `PK` | ID | int |
|--------|--------|:--------:|
|  | Nombre | nvarchar(100) |
| `FK1`  | Id_Pais  | int |
|  | Población | int |
  

### Pais
  
| `PK` | ID | int |
|--------|:--------|:--------:|
|  | Nombre | nvarchar(100) |
|  | Continente  | nvarchar(100) |
|  | PBI | int |
  
Note que existe una relacion entre *`FK1` - Id_pais* de la tabla Ciudad y *`PK`- ID* de la tabla Pais
  
<br>

## Con dichas tablas construya las siguientes queries:
### **5) Calcule la población de todas las ciudades de Asia.**
<br>
  
__Respuesta Esperada__:
```sql
SELECT SUM(Ciudad.Poblacion)
FROM Pais
JOIN Ciudad
ON Pais.ID = Ciudad.Id_pais
WHERE Pais.Continente = 'Asia';
```


### **6) Se debe agregar una ciudad llamada "Springfield" en USA (Id=3320), de población: 50720. Actualice la tabla correspondiente**
<br>
  
__Respuesta Esperada__:
```sql
INSERT INTO Ciudad (Nombre, Id_pais,Poblacion)
VALUES ("Springfield", 3320,50720)
```

  
