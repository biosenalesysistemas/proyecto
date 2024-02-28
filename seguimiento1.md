<p><img alt="udeA logo" height="150px" src="https://github.com/freddyduitama/images/blob/master/logo.png?raw=true" align="left" hspace="50px" vspace="0px" style="width:107px;height:152px;"></p>
<h1><font color='0B5345'> <center>
Seguimiento 1: Análisis exploratorio de datos de EMG</center></font></h1>
<h2><font color='0B5345'> <center>
Proyecto 2024</center></font></h2>
<h3><font color='0B5345'> <center>
John Fredy Ochoa Gómez - Juliana Moreno Rada- Luisa María Zapata Saldarriaga </center></font></h3>
<h3><font color='0B5345'> <center>
2024 </center></font></h3>
<font  face="Courier New" size="3">
<p1><center> </center></p1>

# Seguimiento 1

## Objetivos
  * Aprender a usar Python para la manipulación y visualización básica de señales
  * Programar operaciones matemáticas sobres señales
  * Conocer el efecto de transformaciones sobre las señales en la obtención de índices relevantes en tareas de clasificación
  * Hacer comparaciones e inferencias sobre conjuntos de datos

## Enunciado

Con este proyecto se habilita el acceso a un conjunto de datos de EMG  en dónde se registraron patrones a partir de una pulsera MYO Thalmic que se lleva en el antebrazo del usuario y una PC con un receptor Bluetooth. La pulsera está equipada con ocho sensores equidistantes alrededor del antebrazo que captan simultáneamente señales miográficas. Las señales se envían a través de una interfaz Bluetooth a una PC.

La base de datos de EMG se encuentran los archivos sin procesar de 36 sujetos mientras realizaban series de gestos estáticos con las manos. El sujeto realiza dos series, cada una de las cuales consta de seis (siete) gestos básicos. Cada gesto se realizó durante 3 segundos con una pausa de 3 segundos entre gestos.

### Descripción del archivo raw_data

Cada archivo consta de 10 columnas:
  1) Tiempo: tiempo en ms
  2-9) Canal: ocho canales EMG del brazalete MYO Thalmic
  10) Clase – la etiqueta de los gestos:
    0 - datos no marcados,
      
    1 - mano en reposo,
    
    2 - mano cerrada en un puño,
    
    3 - flexión de muñeca,
    
    4 - extensión de muñeca,
    
    5 - desviaciones radiales,
    
    6 - desviaciones cubitales,
    
    7 - palma extendida (el gesto no fue realizado por todos los sujetos).

Ver más información del dataset aquí: https://www.kaggle.com/datasets/sojanprajapati/emg-signal-for-gesture-recognition

### Medidas 

1. Crear una función que reciba la señal de EMG y permita aplicar el operador Teager-Kaiser Energy Operator (TKEO). (10 %)
   ![image](https://github.com/biosenalesysistemas/proyecto/assets/157903370/6da85b8a-aa90-446a-aa53-5eab5d5a1a83)
2. Crear una función que reciba una señal EMG de múltiples canales y calcule el operador TKEO para cada canal. (10 %)
3. Crear una función que reciba una señal EMG de múltiples canales que extraiga las siguientes características para cada canal (10 %):
   -  RMS
   -  Varianza
   -  Mean Absolute Value
   -  Mean Absolute Value Slope
   -  Slope Sign Changes
   -  Wave form length
   -  Zero Crossing
4. Crear una rutina que aplique sobre todo los archivos de la base de datos las funciones descritas en 2 y 3 (5 %)
5. Crear una rutina que aplique sobre todo los archivos de la base de datos las función 3 sobre las señales originales (5 %)
6. Almanecene las métricas obtenidas en el ítem 4 y 5 en un dataframe, en donde haya una columna que discrimine si las caracteristicas proviene de una señal con TKEO o sin TKEO. (10 %)
7. Realice un análisis exploratorio de los datos (Estadística descriptiva) teniendo como base la teoría vista en clase (Diagramas de cajas, gráficos, medidas de tendencia central) (10 % )

### Informe
Entregar un informe en un Notebook que contenga las funciones diseñadas y la siguiente información: 

a. Hacer un breve resumen sobre la electromiografía y las características de esta señal. (5 %)

b. Hacer una breve descripción del operador de TKEO, que información entrega y como se interpreta con los datos entregados (5%).

c. Discusión  de  las  diferencias  en  los  grupos  usando  las  gráficas  obtenidas. Seleccione el   tipo   de representación que mejor le permita describir la información (10%)

d. Planteamiento de las hipótesis nulas y alternativas (5%), selección del tipo de prueba (paramétrica o no paramétrica) (5%) y discusión de los resultados (10%).

e. El informe debe tener conclusiones de todos los análisis realizados, sin el apartado de conclusiones no se revisa.

### Observaciones 
* Se  recomienda  guardar  los  cálculos  intermedios  que  se  vayan  realizando  sobre  los datos
* Los  cálculos  deben  estar optimizados  siguiendo  el  esquema  vectorial  del  numpy (evitar for innecesarios)
* La nota del trabajo se define en la sustentación. Trabajo sin sustentación tiene como nota final 0.
* Tenga en cuenta, que cada media hora de retraso en la entrega penalizará con un 0.5 de la respectiva nota.
 

## Referencias

Solnik S, Rider P, Steinweg K, DeVita P, Hortobágyi T. Teager-Kaiser energy operator signal conditioning improves EMG onset detection. Eur J Appl Physiol. 2010 Oct;110(3):489-98. doi: 10.1007/s00421-010-1521-8. Epub 2010 Jun 5. PMID: 20526612; PMCID: PMC2945630.


