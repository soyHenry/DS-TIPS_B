# Henry - TIPS Grupo B

## **Cuestionario**:
### **1) Explique que es un iterador y ejemplifique con iteradores de python.**  
__Respuesta Esperada__:   _Un ITERADOR es un objeto que permite recorrer uno a uno los elementos almacenados en una estructura de datos, y operar con ellos. Ejemplos de iteradores de python: Estructura While, Estructura For_ 

### **2) ¿Cuál es la diferencia entre aprendizaje supervisado y aprendizaje no supervisado?.**
__Respuesta Esperada__:   _El aprendizaje supervisado requiere entrenamiento con los datos etiquetados. Por ejemplo, (y al contrario del aprendizaje automático), para realizar un algoritmo de clasificación deberá primero etiquetar los datos que utilizará para entrenar el modelo. Además, en el aprendizaje no supervisado, no existe un conjunto de datos de entrenamiento y sus resultados son desconocidos._
 

### **3) Se lanzan dos dados al aire y se anota la suma de puntos obtenidos. Se pide:**  
**a.La probabilidad de que salga 7.**
__Respuesta Esperada__:  
_Casos Favorables: 6 (1+6),(2+5),(3+4)..._  
_Casos Posibles: 6**2 = 36_
_Probabilidad = 6/36 = 0.1666..._
**b.La probabilidad de que el número obtenido sea par.**  
__Respuesta Esperada__:  
_Casos posibles: 36_  
_Casos Favorables: 18_  
_Probabilidad= 18/36 = 0.5_

### **4) Que diferencia existe entre un Merge y un Join en pandas?**  
__Respuesta Esperada__:  
|  | Merge | Join |
|------|------|-------|
|Estructura|realiza una fusión en la columna que es común en ambos df|realiza su operación de unión a través del índice |
| Fusión | a través de claves o columnas comunes | A través de indices |
| Unión  | Inner Join por defecto  | Left Join por defecto|


### **5) Utilice el contenido del archivo "sqltest.ipynb" para cargarlo en MySQL Workbench**  
**Una vez creada la base de datos realice las siguientes consultas:**  
**a. Lista el nombre de los productos, el precio en euros y el precio en dólares. (1 USD = 300 ARS, 1 EUR = 307 ARS)**  
SELECT nombre AS "nombre de producto", precio/300 AS PrecioUSD, precio/307 AS PrecioEUR   
FROM producto;  
  
  
**b. Lista el nombre de todos los fabricantes en una columna, y en otra columna obtenga en mayúsculas los dos primeros caracteres del nombre del**  **fabricante.**  
__Respuesta Esperada__:  
SELECT nombre, UPPER(LEFT(nombre,2))  
FROM fabricante;  


**c. Lista los nombres y los precios de todos los productos de la tabla producto, redondeando el valor del precio.**  
__Respuesta Esperada__:  
SELECT nombre, ROUND(precio)   
FROM producto;  

 
**d. Lista el nombre y el precio del producto más barato. (Utilice solamente las cláusulas ORDER BY y LIMIT)**    
__Respuesta Esperada__:     
SELECT nombre, precio   
FROM producto   
ORDER BY precio ASC LIMIT 1;

**e. Devuelve una lista con 2 filas a partir de la cuarta fila de la tabla fabricante. La cuarta fila también se debe incluir en la respuesta.**  
SELECT *   
FROM fabricante  
LIMIT 3,2;
