# Practica-profesionalizante
Proyecto sobre una empresa del sector educativo. Voy a simular una academia o instituto que ofrece cursos y analizar su actividad para:

1) Explorar el comportamiento de las inscripciones.
2) Predecir cuántas inscripciones tendrá en el futuro.
3) Optimizar el proceso educativo y comercial (ej.: mejorar tasas de inscripción, reducir abandonos, etc.)


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

Vamos a construir un modelo predictivo de clasificación que intente predecir si un alumno finalizará el curso o no, basándonos en sus características.

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

Vamos a usar un Árbol de Decisión (DecisionTreeClassifier) por ser fácil de interpretar y adecuado para datos categóricos mezclados con numéricos.
