# Practica-profesionalizante
Proyecto sobre una empresa del sector educativo. Voy a simular una academia o instituto que ofrece cursos y analizar su actividad para:

1) Explorar el comportamiento de las inscripciones.
2) Predecir cuántas inscripciones tendrá en el futuro.
3) Optimizar el proceso educativo y comercial (ej.: mejorar tasas de inscripción, reducir abandonos, etc.)


# 🎓 Análisis Exploratorio y Modelado Predictivo – Academia Educativa

Este proyecto desarrolla un **Análisis Exploratorio de Datos (EDA)** y **modelos predictivos supervisados** aplicados a un dataset institucional de una academia educativa.  
Se busca comprender los factores que influyen en la finalización de los cursos, la efectividad de los canales de difusión y los perfiles de estudiantes con mayor riesgo de abandono.

---

## 📂 Archivos principales

| Archivo | Descripción |
|----------|--------------|
| `dataset_academia_educativa_var_coords.csv` | Dataset base del proyecto, con variables académicas, demográficas y geográficas. |
| `PP.ipynb` | Notebook principal con el análisis EDA, KPIs, modelos predictivos y conclusiones. |

---

## 🧩 Estructura del dataset

El dataset combina información de inscripción y desempeño de alumnos en diferentes cursos de una academia.

| Columna | Descripción |
|----------|--------------|
| `nombre_curso` | Nombre del curso o programa. |
| `modalidad` | Modalidad de cursado (`Presencial`, `Virtual`). |
| `genero` | Género declarado del estudiante. |
| `region` | Provincia o región de procedencia. |
| `medio_publicidad` | Canal por el cual se enteró del curso (Instagram, Facebook, Google, etc.). |
| `edad` | Edad del estudiante. |
| `fecha_inscripcion` | Fecha de inscripción en el curso. |
| `precio` | Valor del curso en pesos argentinos. |
| `duracion_semanas` | Duración total del curso. |
| `calificacion_final` | Nota final obtenida (0 a 10). |
| `finalizo` | Indicador binario (`Sí` / `No`) que señala si completó el curso. |
| `Latitud`, `Longitud` | Coordenadas geográficas aproximadas para visualización geoespacial. |

---

## 🔍 Etapas del análisis (EDA)

La notebook desarrolla un **EDA completo**, incluyendo:

1. **Inspección estructural del dataset**  
   - Tipos de variables, valores faltantes, duplicados y outliers.
2. **KPIs institucionales**  
   - Tasa de finalización, promedio de calificaciones, curso más elegido, canal más efectivo, diferencias por modalidad.
3. **Distribuciones y relaciones clave**  
   - Análisis descriptivo de edad, modalidad, género, región y desempeño.
4. **Preparación del dataset para modelado**  
   - Encoding categórico, división train/test y balanceo de clases.

---

## 🤖 Modelado predictivo

Se desarrollaron modelos de clasificación para predecir la **probabilidad de finalización** de los alumnos:

| Modelo | Descripción | Resultado (F1_macro) |
|---------|--------------|----------------------|
| **Regresión Logística** | Modelo lineal base, interpretable y robusto. | Medio |
| **Random Forest** | Ensamble de árboles con manejo de no linealidades y alta precisión. | Alto |
| **XGBoost** *(opcional)* | Variante optimizada con boosting. | Muy alto (si instalado) |

Métricas evaluadas:
- Accuracy
- Balanced Accuracy
- F1-score (macro)
- Matriz de confusión
- Clasification report

---

## 💡 Resultados e interpretaciones

- La **modalidad** y el **medio de publicidad** son variables altamente asociadas a la finalización.  
- Se detectaron canales con **alto volumen pero baja conversión**, útiles para optimización de marketing.  
- Los modelos permiten estimar un **riesgo de abandono**, priorizando acciones preventivas (contacto, tutorías).  
- Se generó un **reporte ejecutivo automatizado** con KPIs, análisis por canal y recomendaciones de acción.

---

## 🧭 Recomendaciones estratégicas

1. Reforzar la inversión en los canales con **alta conversión y volumen** (Instagram, Google Ads).  
2. Implementar tutorías y contacto proactivo en segmentos con **alto riesgo de abandono**.  
3. Mantener un equilibrio entre cursos **virtuales y presenciales** según la demanda real.  
4. Utilizar el modelo predictivo como herramienta de **alerta temprana** para gestión académica.

---

## ⚙️ Requisitos técnicos

Para ejecutar la notebook se requieren las siguientes librerías (Python 3.10+):

```bash
pip install pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost y plotly.

## 📊 Visualización del Proyecto

Para complementar el análisis de datos, se desarrolló un dashboard interactivo en Tableau que permite explorar visualmente los principales resultados del proyecto.

🔗 Ver dashboard interactivo:  
https://public.tableau.com/views/PP_17635695435420/Dashboard2?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

El dashboard permite:
- Visualizar métricas clave del análisis.
- Explorar patrones y tendencias en los datos.
- Facilitar la interpretación de los resultados obtenidos en el proyecto.

La visualización fue desarrollada utilizando **Tableau Public**.

<img width="2034" height="1143" alt="Dashboard 2" src="https://github.com/user-attachments/assets/065ea941-d57a-4e04-87f7-cce0d387e34e" />
