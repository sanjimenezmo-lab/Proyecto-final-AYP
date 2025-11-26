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

## Características del Dataset

### Valores faltantes
- Algunas columnas como Item, Payment Method o Location contenían valores vacíos o nulos.

### Valores inválidos
- Se incluían entradas como "ERROR", "UNKNOWN" o números en formatos incorrectos.

###  Coherencia económica
- Los precios por producto siguen rangos definidos (ej. Coffee → $2).

### Elementos incluidos en el menú

| Ítem | Precio ($) |
|------|------------|
| Coffee | 2 |
| Tea | 1.5 |
| Sandwich | 4 |
| Salad | 5 |
| Cake | 3 |
| Cookie | 1 |
| Smoothie | 4 |
| Juice | 3 |

---

## Uso propuesto del Dataset
El dataset es ideal para practicar:

- Limpieza de datos (missing values, valores inválidos, normalización).  
- Manipulación con Pandas.  
- Feature engineering.  
- Exploratory Data Analysis (EDA).  

---

## ¿Qué se hizo en este proyecto?

En este trabajo se realizaron las siguientes etapas:

### *1. Carga e inspección del archivo*
- Se importó el CSV en Google Colab.
- Se revisaron tipos de datos, dimensiones y estructura general.

### *2. Limpieza profunda*
- Reemplazo de valores inválidos (ERROR, UNKNOWN, None).
- Conversión de tipos (fechas, números, categorías).
- Normalización de campos categóricos.
- Reconstrucción y validación del cálculo *Total Spent = Quantity × Price Per Unit*.
- Creación de columnas derivadas:
  - Transaction Month
  - Transaction Weekday
  - expected_total
  - price_diff (para validar coherencia)

### *3. Análisis Exploratorio (EDA)*
- Resúmenes estadísticos.
- Distribuciones de cantidad, precios y montos gastados.
- Análisis temporal por mes y por día de la semana.
- Detección de patrones y comportamiento del cliente.

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
