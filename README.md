# Practica-profesionalizante
Proyecto sobre una empresa del sector educativo. Voy a simular una academia o instituto que ofrece cursos y analizar su actividad para:

1) Explorar el comportamiento de las inscripciones.
2) Predecir cuántas inscripciones tendrá en el futuro.
3) Optimizar el proceso educativo y comercial (ej.: mejorar tasas de inscripción, reducir abandonos, etc.)

🧠 Proyecto: 
"Optimización de Procesos Educativos a través del Análisis Predictivo de Datos de Inscripción"

"Proyecto de Ciencia de Datos para la Optimización de Cursos en una Plataforma Educativa"

Este proyecto incluirá:

Análisis Exploratorio de Datos (EDA)

Modelos Predictivos

Optimización de Procesos

✅ Paso 1: Definición del Alcance del Proyecto

📌 Nombre del Proyecto:
“..............”

🎯 Objetivos:

Objetivo	          Detalle
EDA	                 Explorar los datos históricos de ventas para conocer                          patrones y tendencias
Predicción	          Predecir las ventas del próximo mes (o trimestre)
Optimización	         Detectar productos de baja rotación, demoras                                  logísticas o ineficiencias comerciales y proponer                              mejoras

✅ Paso 2: Dataset (real o simulado)

📚 Educación (inscripciones, cursos)


✅ Paso 3: Herramientas que vamos a usar
Python (pandas, matplotlib, seaborn, scikit-learn)

Visual Studio Code 
Power BI / Tableau

Informe final en Word o PDF

✅ Paso 4: Entregables del Proyecto

Dataset limpio y procesado

Análisis Exploratorio de Datos

Modelo Predictivo (regresión lineal o árbol de decisión)

Informe con propuestas de mejora en procesos

Dashboard o visualización 

## 🔧 Etapas del Proyecto

🔹 1. Análisis Exploratorio de Datos (EDA)

¿Cuáles son los cursos más elegidos?

¿Cuál es la tasa de finalización por curso?

¿Cuál es el promedio de edad por curso o modalidad?

¿Cuál es el canal de publicidad más efectivo?

🔹 2. Modelo Predictivo

Predicción 1: ¿Se puede predecir si un alumno terminará el curso?

Modelo: Clasificación (por ejemplo, Regresión Logística o Árbol de Decisión)

Predicción 2: ¿Cuántos alumnos se inscribirán el mes siguiente?

Modelo: Regresión sobre series temporales (si simulamos varios meses/años)

🔹 3. Optimización de Procesos

¿Conviene invertir más en cierto canal de publicidad?

¿Hay cursos con alta deserción que podrían mejorarse?

¿Qué modalidad funciona mejor en cada región?




### DESARROLLO
🔹 2. Modelo Predictivo

Voy a construir un modelo predictivo de clasificación que intente predecir si un alumno finalizará el curso o no, basándome en sus características.

🔍 Objetivo del Modelo

Variable objetivo (y): finalizo (Sí / No)
Variables predictoras (X):

nombre_curso

modalidad

duracion_semanas

precio

edad

genero

region

medio_publicidad

⚙️ Modelo Sugerido

Voy a usar un Árbol de Decisión (DecisionTreeClassifier) por ser fácil de interpretar y adecuado para datos categóricos mezclados con numéricos.
