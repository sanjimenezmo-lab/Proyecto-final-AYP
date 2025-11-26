# Proyecto de Gestión de Datos y Análisis Hospitalario

##  Descripción del Proyecto  
Este proyecto consiste en un proceso integral de Ingeniería de Datos y Análisis Biomédico aplicado a un conjunto de datos hospitalarios. El objetivo principal fue transformar datos crudos en información accionable para la toma de decisiones clínicas y administrativas.

El trabajo se desarrolló en [**Google Colab**](https://colab.research.google.com/drive/16E0WffiXZ6UXxcDjH5p97sQ-x0zf3MKk?usp=sharing), utilizando **Python**, **Pandas**, **NumPy** y otras librerías del ecosistema científico.

El resultado final es una base de datos completamente limpia, estructurada y lista para análisis más avanzados, como visualizaciones, modelos descriptivos o modelado predictivo.

---

## Información del Dataset

El dataset Healthcare Dataset contiene 55,500 registros sintéticos que simulan la operación de un sistema hospitalario moderno. Su estructura balanceada lo hace ideal para ejercicios de gestión sanitaria, modelado predictivo y análisis de eficiencia.
El database se pude visualizar [aquí](https://www.kaggle.com/datasets/prasad22/healthcare-dataset)

### Archivo incluido
- *Nombre:* healthcare_dataset.csv
- *Filas:* 55500
- *Columnas:* 15  

###  Descripción de Columnas

| Columna            | Descripción | Ejemplo |
|--------------------|-------------|---------|
| *Medical Condition* | Patología diagnosticada al paciente. | Cancer, Obesity, Diabetes |
| *Date of Admission* | Fecha de ingreso al hospital. | 2024-01-31 |
| *Discharge Date* | Fecha de alta médica. | 2024-02-02 |
| *Billing Amount* | Monto total facturado por el tratamiento. | 18856.3 |
| *Doctor* | Médico tratante responsable. | Matthew Smith |
| *Hospital* | Centro médico donde se realizó la atención. | Sons and Miller |
| *Medication* | Medicamento principal prescrito. | Paracetamol, Ibuprofen |
| *Test Results* | Resultado de las pruebas clínicas. | Normal, Abnormal |

---

## Metodología y Procesamiento de Datos

### Revisión previa a limpieza
Se realizó una inspección técnica inicial que reveló:
- Registros Duplicados: Se identificaron y eliminaron 534 registros redundantes para evitar sesgos estadísticos.

### Inconsistencias Lógicas
- Detección de valores negativos en la columna Billing Amount, los cuales fueron corregidos aplicando valor absoluto.

###  Estandarización
- Normalización de nombres propios y formatos de texto.



---

## Uso propuesto del Dataset
El dataset es ideal para practicar:

- Limpieza de datos (missing values, valores inválidos, normalización).  
- Manipulación con Pandas.  
- Feature engineering.  
- Exploratory Data Analysis (EDA).  

---

## Ingeniería de Características 

Para profundizar el análisis, se creó una nueva variable crítica:

### *Length of Stay (LOS): Calculada como la diferencia entre la fecha de alta y la fecha de ingreso. Esta métrica es el estándar de oro para medir la eficiencia en la gestión de camas hospitalarias.*


## * Análisis Exploratorio (EDA) con Enfoque Biomédico*

### Se generaron visualizaciones técnicas (sin distracciones visuales) para responder preguntas de negocio:

- Eficiencia Operativa: Análisis de la distribución de días de estancia por patología.
- Gestión Financiera: Evaluación de costos promedio y totales por tipo de enfermedad.
- Cadena de Suministro: Identificación del medicamento más prescrito (moda) para cada condición médica.
- Recursos Humanos: Ranking de carga laboral por médico para optimización de turnos.

### *Hallazgos Clave del Análisis*

- Uniformidad Operativa: La distribución de pacientes por patología y tipo de ingreso es notablemente equilibrada, sugiriendo un modelo de demanda estable.
- Estandarización de Protocolos: El promedio de días de estancia (LOS) se mantiene constante alrededor de 15.5 días para todas las condiciones, indicando protocolos de recuperación altamente estandarizados.
- Modelo de Costos: Se encontró una correlación nula entre los días de estancia y el monto facturado. Esto sugiere que el hospital opera bajo un modelo de facturación por procedimiento (tipo GRD) y no por día-cama.
- Estabilidad Financiera: Los costos promedio de tratamiento son homogéneos entre las diferentes enfermedades (~$25,500), facilitando la previsión presupuestaria.

### *4. Exportación final*
- Se generó un CSV totalmente limpio y listo para nuevos análisis o modelos.
- También se creó un PDF con un resumen del proyecto.

---

##  Licencia del Dataset
El dataset fue publicado bajo *CC BY-SA 4.0*, lo cual permite:
- Usarlo  
- Modificarlo  
- Compartirlo  
Siempre que se dé crédito al creador original.

---

## Tecnologías Utilizadas
- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Google Colab  

---
