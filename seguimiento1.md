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
-Aprender a usar Python para la manipulación y visualización básica de señales
-Programar operaciones matemáticas sobres señales
-Hacer comparaciones e inferencias sobre conjuntos de datos

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

### Aspectos generales dela señal 
  - Los datos fueron tomados con una frecuencia de muestre fs =
  - 
