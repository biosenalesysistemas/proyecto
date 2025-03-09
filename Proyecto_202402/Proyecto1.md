<p><img alt="udeA logo" height="150px" src="https://github.com/freddyduitama/images/blob/master/logo.png?raw=true" align="left" hspace="50px" vspace="0px" style="width:107px;height:152px;"></p>
<h1><font color='0B5345'> <center>
Proyecto 1: Análisis estadístico</center></font></h1>
<h2><font color='0B5345'> <center>
Proyecto 2024-02 </center></font></h2>
<h3><font color='0B5345'> <center>
John Fredy Ochoa Gómez - Juliana Moreno Rada- Luisa María Zapata Saldarriaga </center></font></h3>
<h3><font color='0B5345'> <center>
2024 </center></font></h3>
<font  face="Courier New" size="3">
<p1><center> </center></p1>

## Contexto del problema
Las enfermedades neurodegenerativas a menudo afectan la marcha y la movilidad. Para comprender mejor la fisiopatología de estas enfermedades y mejorar nuestra capacidad de medir las respuestas a las intervenciones terapéuticas, puede resultar útil cuantificar con precisión la dinámica de la marcha (https://physionet.org/content/gaitndd/1.0.0/).

## Objetivos proyecto
- Fortalecer las competencias en programación para el análisis de datos
- Discutir resultados a partir de gráficos y estadística descriptiva
- Evaluar el impacto de la extracción de características de señales para encontrar patrones diferenciales en datos de poblaciones clínicas
- Proponer nuevas estrategias de análisis de información fisiológica para el diseño de ayudas diagnósticas

## Origen de los datos
Gait in Neurodegenerative Disease Database v1.0.0 (physionet.org)

Los registros de esta base de datos provienen de pacientes con **enfermedad de Parkinson** (n = 15), **enfermedad de Huntington** (n = 20) y **esclerosis lateral amiotrófica** (n = 13). Aquí también se incluyen registros de 16 sujetos de control sanos.

De los archivos (.ts) se analizarán las señales:

| Columna  |Contenido|
|---|---|
|1|Tiempo transcurrido (sec) - Útil para graficar las señales en escala|
|2|Intervalo entre pasos píe izquierdo (sec)|
|3|Intervalo entre pasos píe derecho (sec)|
|4|Intervalo balanceo píe izquierdo (sec)|
|5|Intervalo balanceo píe derecho (sec)|

## **Requerimientos**
### **Contexto**
• Consultar para enfermedad de Parkinson, Huntington y Esclerosis Lateral Amiotrófica cómo se diagnostican y el reto que existe para el diagnóstico temprano de dichas enfermedades **(5%).**
• Discutir matemáticamente, explicando con fórmulas, cómo funciona la rutina detrend de scipy **(5%)**
• Discutir matemáticamente, explicando con fórmulas, cómo funciona el filtro hampel **(5%)**
• Discutir matemáticamente y desde la bioingeniería qué mide la entropia de permutación ( https://www.aptech.com/blog/permutation-entropy/ , https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8051436/ ) **(5%)**

### **Organización de la base de datos**

Organizar los datos en carpetas de acuerdo al tipo de población almacenando los archivos .ts para Parkinson, otra para Huntington, Esclerosis Lateral Amiotrófica, Controles

### **Programación**

1. Crear una rutina que permita cargar un archivo .ts y extraiga las 4 señales de interés, de cada señal elimine los primeros 20 segundos, y las almacene en un ndarray.
2. Para cada señal eliminar los errores en tendencia usando la rutina detrend.
3. Para cada señal resultante del paso 2 eliminar los datos atípicos usando filtro hampel
4. Crear una función que reciba una señal de marcha y calcule el coeficiente de variación (CV) y la SD tal como se define en el artículo de referencia .
5. Crear una función que reciba una señal de marcha y permita calcular la entropía de permutación **(10%)**
6. Crear una rutina que aplique sobre todos los archivos de la base de datos las rutina 1 y almacene los resultados en un dataframe donde se pueda discriminar nombre participante, condición (Parkinson, Huntington, ELA, Control) y los tres índices/características calculados por cada señal

| Sujeto|Estado|ent_intervalo_izq|...|ent_balanceo_der|cv_intervalo_izq|
|---|---|---|---|---|---|
| x | x  | x  | x  | x  | x  |
| x | x  |  x |  x |  x | x  |

**Entregar un informe con:**

a. Discusión de las diferencias en los grupos usando las gráficas obtenidas usando estadística descriptiva **(25%)**
b. Planteamiento de las hipótesis nulas y alternativas **(5%)**, selección del tipo de prueba (paramétrica o no paramétrica) **(10%)** y discusión de los resultados **(10%)**
c. Discutir los resultados obtenidos con los presentado en el artículo base **(10%)**
d. Proponer cuales de las medidas usadas podrían servir para discriminar que poblaciones clínicas de los controles **(10%)**
