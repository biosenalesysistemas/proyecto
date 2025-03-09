<p><img alt="udeA logo" height="150px" src="https://github.com/freddyduitama/images/blob/master/logo.png?raw=true" align="left" hspace="50px" vspace="0px" style="width:107px;height:152px;"></p>
<h1><font color='0B5345'> <center>
Proyecto 2 : Análisis de señales ECG</center></font></h1>
<h2><font color='0B5345'> <center>
Proyecto 2024-02 </center></font></h2>
<h3><font color='0B5345'> <center>
John Fredy Ochoa Gómez - Juliana Moreno Rada- Luisa María Zapata Saldarriaga </center></font></h3>
<h3><font color='0B5345'> <center>
2024 </center></font></h3>
<font  face="Courier New" size="3">
<p1><center> </center></p1>

Las enfermedades cardiovasculares son una de las principales causas de muerte en todo el mundo, y la Organización Mundial de la Salud (OMS) estimó que 17,9 millones de personas murieron en 2019 por este tipo de enfermedades. Las enfermedades cardiovasculares están relacionadas con problemas de salud que afectan el corazón y los vasos sanguíneos. El riesgo de estas enfermedades aumenta con el tabaquismo, la presión arterial alta, el colesterol alto, una dieta poco saludable, la falta de ejercicio y la obesidad. 

El uso de la tecnología puede mejorar los tratamientos sanitarios y el seguimiento con la ayuda de diferentes sensores disponibles en los dispositivos que son cada vez de mayor uso. También, debido al bajo costo de algunos dispositivos de Electrocardiografía (ECG), el personal de salud puede tener a disposición la medición de la actividad eléctrica cardiaca. 

Parámetros fisiológicos como la frecuencia cardíaca, la presión arterial y la temperatura corporal que se miden habitualmente en entornos clínicos son muy relevantes, pero estos parámetros tienen alta variabilidad por lo que se requieren mediciones en grandes conjuntos de sujetos de manera que se capture dicha variabilidad para la construcción de modelos.  

Sin embargo, el avance en el uso de las bioseñales implica tener los diferentes conjuntos de datos relacionados con diversas enfermedades cardiovasculares debidamente procesadas y etiquetadas , implicando la necesidad de analizar proyectos como MIT-BIH o en Physionet, para disponer de la cantidad de datos necesarios para construir modelos con alto poder diagnóstico o predictivo. El enfoque de grandes volúmenes de datos también permite validar los procedimientos de procesamiento y análisis en diferentes poblaciones y tecnologías aumentando la pertinencia de las tecnologías desarrolladas. 

Un electrocardiograma (ECG) es un registro de la actividad eléctrica del corazón. Se usa ampliamente en entornos clínicos para detectar afecciones cardiovasculares, como ataques cardíacos y alteraciones del ritmo que cambian la actividad eléctrica del corazón. Un ECG se mide colocando electrodos en el pecho y las extremidades de un paciente, que registran diferentes aspectos de la actividad eléctrica de su corazón, y cada aspecto está etiquetado como una derivación. 

Un ECG convencional consta de 12 derivaciones, que proporcionan una visión completa de la actividad eléctrica del corazón. Seis de las derivaciones se obtienen colocando cuatro electrodos, uno en cada extremidad, proporcionando las derivaciones I, II, III, VL, VF y VR. Se colocan seis electrodos en el tórax, que proporcionan los cables V1 a V6. La derivación de aplicación más inmediata es la II. La amplitud de la señal del ECG está dentro del rango de 10 V a 4 mV. La frecuencia más importante de esta señal se encuentra dentro del rango de 0,05 a 100 Hz.  

 

**Entregable**

1. De los artículos: 

- https://www.nature.com/articles/s41746-023-00966-w  

- https://www.nature.com/articles/s41598-020-59821-7 

- https://www.sciencedirect.com/science/article/pii/S2405844024032316 

Para cada artículo hacer un diagrama de flujo de las metodologías usadas en los artículos (10%) 

Explicar en sus palabras las metodologías desarrolladas **(10%)**

2. Descargar los datos ECGDataDenoised.zip de:  

https://figshare.com/collections/ChapmanECG/4560497/1  

De la base de datos extraer los registros que correspondan a bradicardia sinusal (SB Sinus Bradycardia) y fibrilación auricular (AFIB Atrial Fibrillation). Esta información está en el archivo Diagnostics.xlsx 

De la base de datos extraer los registros que correspondan a bradicardia sinusal (SB Sinus Bradycardia) y fibrilación auricular (AFIB Atrial Fibrillation). Esta información está en el archivo Diagnostics.xlsx 

![image](https://github.com/user-attachments/assets/ab9a1334-cdf8-475e-b67e-76c1f92e1db5)

**De estos registros los análisis para el presente proyecto deben hacerse en la derivación II** 

3. Programar las fórmulas 1 al 4 que se encuentran en el artículo **(15%)**. Consultar que significado y utilidad del biespectro (Realice la gráfica) **(5%)** 

- https://arxiv.org/pdf/1809.08451

4. Para cada señal extraer la frecuencia que contiene la máxima potencia y Gráfiquela **(15%)** 

5. Para cada señal sumar el número de frecuencias que son significativas para bicoherencia (cuales tienen un valor superior a ![image](https://github.com/user-attachments/assets/636a4170-c3f7-4789-9100-f2a0ce0033c3)
 **(20%)** 

 6. Crear una rutina que aplique sobre todos los archivos de la base de datos las rutina 3 al 5 y almacene los resultados en un dataframe donde se pueda registro, tipo de patología y el frecuencia de máxima potencia (fMP) y suma de frecuencias significativas en bicoherencia (sFSB): 


| Registro | Estado | fMP | sFSB  |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |



7. Para las señales de análisis del punto 2 aplicar las rutinas del punto 3 al 5 y hacer un informe que permita **evidenciar** las diferencias entre las señales SB y AFIB utilizando las herramientas de estadística descriptiva **(5%)** 

8. Indicar si hay o no diferencias estadísticas entre las características espectrales del punto 4 y 5 para las dos poblaciones de estudio **(5%)** 

9. Hacer un informe con todos los puntos anteriores **(15%)** 

 **Trabajo sin sustentar no se califica**

 


