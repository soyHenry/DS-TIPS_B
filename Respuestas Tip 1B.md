<h1>TIPS: Technical Interview Preparation</h1>
<h2>Grupo B --&gt; Primer Set de Tips con Respuestas</h2>
<h2>NO MOSTRAR A SUS PAREJAS DE TIPS!</h2>
<h3>1)  Respuesta:</h3>
<p>Una subconsulta es una consulta hecha sobre otra consulta.</p>
<p>SELECT <column_name> FROM <table_name> </p>
<p>WHERE <column_name> IN/NOT IN </p>
<p>(subconsulta)</p>
<h3>2)  Respuesta:</h3>
<p>Hay muchas. Entre las más utilizadas para realizar visualizaciones varias está matplotlib (de muy bajo nivel), seaborn (construida sobre matplotlib), plotly (muy completa y de alto nivel, permite simplificar mucho la sintaxis para realizar gráficos interactivos pero es computacionalmente más costosa), plotnine (muy similar a ggplot2 muy usado en el lenguaje R), Gleam (muy similar a Shiny en el lenguaje R), missingno (muy útil para lidiar con datos faltantes), leather (permite generar gráficos simples pero en formato SVG muy escalables a cualquier resolución), Bokeh (permite gráficos interactivos) y Altair (permite gráficos interactivos muy llamativos). Para mapas, pueden utilizar Plotly, Bokeh, Altair, la librería Folium permite crear mapas interactivos muy personalizables y computacionalmente más baratos que plotly, también está la librería Geoplotlib. Para los dashboards, se puede utilizar Bokeh, Dash o Streamlit. </p>
<h3>3)  Respuesta:</h3>
<p><code>def tabla_multiplicar(n):
    print("Tabla de multiplicar de", n, ":")
    for i in range(1, 11):
        resultado = n * i
        print(n, "x", i, "=", resultado)
<p>tabla_multiplicar(5)</code> </p>
<h3>4)  Respuesta:</h3>
<p>Pueden implementarse 3 tipos de filtros:</p>
<p>Filtros a nivel visualización: filtra tanto datos como medidas calculadas, limitando la cantidad de información que puede verse en una visualización determinada.</p>
<p>Filtros a nivel página: filtra la info en todas las visualizaciones de una página específica del reporte.</p>
<p>Filtros a nivel reporte: se aplican a todas las páginas y visualizaciones en simultáneo.</p>
<h3>5)  Respuesta:</h3>
<p>i.Casos Favorables: 12
Casos posibles: 8 + 5 + 7 = 20
Probabilidad = Casos Favorables/Casos Posibles= 12/20 = 0.6</p>
<p>ii. Casos Favorables: 13
Casos posibles: 8 + 5 + 7 = 20
Probabilidad = Casos Favorables/Casos Posibles= 13/20 = 0.65</p>
<p>iii. Casos Favorables: 5
Casos posibles: 8 + 5 + 7 = 20
Probabilidad = Casos Favorables/Casos Posibles= 5/20 = 0.25</p>
<h3>6)  Respuesta:</h3>
<p>La regresión lineal es un método estadístico que se utiliza para modelar la relación entre una variable dependiente y una o más variables independientes. La regresión lineal se utiliza para predecir el valor de la variable dependiente en función de los valores de las variables independientes. </p>
