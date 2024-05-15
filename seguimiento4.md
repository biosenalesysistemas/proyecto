<p><img alt="udeA logo" height="150px" src="https://github.com/freddyduitama/images/blob/master/logo.png?raw=true" align="left" hspace="50px" vspace="0px" style="width:107px;height:152px;"></p>
<h1><font color='0B5345'> <center>
Seguimiento 4: Machine Learning  </center></font></h1>
<h2><font color='0B5345'> <center>
Proyecto 2024</center></font></h2>
<h3><font color='0B5345'> <center>
John Fredy Ochoa Gómez - Juliana Moreno Rada- Luisa María Zapata Saldarriaga </center></font></h3>
<h3><font color='0B5345'> <center>
2024 </center></font></h3>
<font  face="Courier New" size="3">
<p1><center> </center></p1>

# Seguimiento 4

De los proyectos anteriores tenemos:
1. Información sobre fisiología de la señal EMG
2. Procesamiento y extracción de características de la señal 
3. Análisis
   
Se solicita entregar un informe con: 

a.	Correcciones del proyecto 1.

b.	(10%) Definir una estrategia de filtrado de las señales del proyecto 1 usando filtros IIR o FIR justificando la selección (10%)

c.	(10%) Obtener los índices del proyecto 1 usando la señal filtrada (Después de aplicar señal TKEO). Comparar los índices obtenidos de la señal filtrada con los obtenidos en el proyecto 1 (Señal con Operador TKEO) usando gráficos de Análisis Exploratorio de Datos (10%)

d.	(10%) Analizar y discutir los resultados del punto anterior de manera que para los puntos siguientes se usen, debidamente sustentado, los índices obtenidos con la señal filtrada o la señal sin filtrar (10%).

**Todos los puntos realizados a continuación son con las características definidas del punto d**

e.	(30%) Código y análisis de resultados, donde se discutan por los menos tres diferentes arquitecturas de red (20%) y las matrices de confusión obtenidas (10%), de una red neuronal que permita la clasificación de los diferentes gestos (Etiquetas con los datos del primer proyecto). 

f.	(25%) Consultar (10%), justificar el uso (5%) e **implementar** otros modelos de machine learning que permitan la clasificación de gestos (10%)

g.	(15%) Discutir cómo se podría implementar la solución del punto e y f usando sistemas embebidos seleccionando el tipo de microcontrolador (5%) y los posibles tiempos de adquisición y clasificación de las señales (10%)

## Observaciones

* Los datos para entrenar el modelo, son los datos utilizados en el primer proyecto 

* Trabajo sin sustentar no se califica
  
* Documentación adicional

## Recomendaciones 

* El dataset de entrada del modelo debe tener los sujetos como filas, y las características como columnas. Recuerden que también debe tener un target (Columna que diferencie la clase) 
* Utilicé para las comparaciones solamente la señal con TKEO

## Referencias
  
* https://scikit-learn.org/stable/modules/neural_networks_supervised.html
  
* https://scikit-learn.org/stable/modules/generated/sklearn.metrics.multilabel_confusion_matrix.html
  
* https://scikit-learn.org/stable/modules/model_evaluation.html#multilabel-confusion-matrix
