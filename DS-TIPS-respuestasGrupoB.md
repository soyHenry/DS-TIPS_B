# Henry - TIPS Grupo B

## **Cuestionario**:
### **1) Explique que es una función de agregación y mencione al menos 5 de las más comunes.**  
__Respuesta Esperada__:   _(Count, AVG, Max, Min, STDDEV, Variance), Las funciones de agregación realizan análisis estadísticos sobre número (o fechas en algunos casos)_ 

### **2) Describa y explique los diferentes tipos de JOINS para SQL.**
__Respuesta Esperada__:   _INNER JOIN: Devuelve todas las filas cuando hay al menos una coincidencia en ambas tablas._ 
                          _LEFT JOIN: Devuelve todas las filas de la tabla IZQUIERDA y las filas coincidentes de la tabla de la derecha._ 
                          _RIGHT JOIN: Devuelve todas las filas de la tabla DERECHA y las filas coincidentes de la tabla de la izquierda._ 
                          _OUTER JOIN: Devuelve todas las filas de las dos tablas. También conocida como FULL OUTER JOIN.._ 


### **3) La probabilidad de que un hombre viva 20 años es de 1/4 y la de que su mujer viva 20 años es de 1/3. Calcular la probabilidad de**  
**a)** Que ambos vivan 20 años.  
__Respuesta Esperada__:   _Note que son sucesos independientes, por lo tanto:_  
Probabilidad = (1/4) . (2/3) = 1/12   
**b)** De que el hombre viva 20 años y la mujer no.      
__Respuesta Esperada__:       
Probabilidad = (1/4) . (1 - (1/3))  
Probabilidad = (1/4) . (2/3) = 1/6  
**c)** De que ambos mueran antes de los 20 años.   
__Respuesta Esperada__:       
Probabilidad = (1 - (1/4)) . (1 - (1/3))  
Probabilidad = (3/4) . (2/3)  
Probabilidad = 1/2 = 0.5  
  
   

  
  

## Suponga tiene la tabla EMPLEADOS compuesta de la siguiente forma:

| IDEmpleado | Nombre | Apellido |
|--------|--------|--------|
| valor | valor | valor |
|valor  | valor  | valor |



### **4) Cree una consulta SQL que obtenga los apellidos de los empleados sin repeticiones**
__Respuesta Esperada__:  
_SELECT DISTINCT Apellido FROM EMPLEADOS_

### **5) Obtener todos los datos de los empleados que se apellidan "López" y los que se apellidan "Gutierrez"**
__Respuesta Esperada__:  

Utilizando OR:  
_SELECT * FROM EMPLEADOS_  
_WHERE Apellido = 'López' OR Apellido = 'Gutierrez'_  

Utilizando IN:  
_SELECT * FROM EMPLEADOS_  
_WHERE Apellido IN ('López', 'Gutierrez')_  
 
### **5) Obtener todos los datos de los empleados cuyo apellido comience con la letra 'P'**
__Respuesta Esperada__:  

_SELECT * FROM EMPLEADOS_  
_WHERE Apellido LIKE 'P%'_
