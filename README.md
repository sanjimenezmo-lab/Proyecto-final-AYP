# Proyecto de Limpieza y Análisis del Dataset Dirty Cafe Sales

## 📌 Descripción del Proyecto  
Este proyecto tiene como objetivo realizar un proceso completo de *limpieza de datos, **transformación, y **análisis exploratorio (EDA)* sobre el dataset Dirty Cafe Sales, un conjunto de datos diseñado específicamente para practicar habilidades de Data Cleaning y Wrangling.  

El trabajo se desarrolló en *Google Colab, utilizando **Python, **Pandas, **NumPy* y otras librerías del ecosistema científico.

El resultado final es una base de datos completamente limpia, estructurada y lista para análisis más avanzados, como visualizaciones, modelos descriptivos o modelado predictivo.

---

## Información del Dataset

El dataset *Dirty Cafe Sales* contiene *10,000 registros* sintéticos sobre transacciones realizadas en un café.  
Fue creado de forma intencionalmente “sucia”, es decir, incluye valores faltantes, inconsistentes y errores comunes en datos reales, con el fin de practicar técnicas de limpieza.

### 📄 Archivo incluido
- *Nombre:* dirty_cafe_sales.csv  
- *Filas:* 10,000  
- *Columnas:* 8  

###  Descripción de Columnas

| Columna            | Descripción | Ejemplo |
|--------------------|-------------|---------|
| *Transaction ID* | Identificador único de la transacción. Siempre presente. | TXN_1234567 |
| *Item* | Producto comprado; puede tener valores faltantes o incorrectos. | Coffee, Sandwich, ERROR |
| *Quantity* | Cantidad comprada; puede incluir valores inválidos. | 1, 3, UNKNOWN |
| *Price Per Unit* | Precio unitario del ítem; puede estar incompleto o errado. | 2.00, 4.00 |
| *Total Spent* | Total pagado (Quantity * Price). | 8.00, 12.00 |
| *Payment Method* | Método de pago; puede contener None o UNKNOWN. | Cash, Credit Card |
| *Location* | Lugar de la compra. | In-store, Takeaway |
| *Transaction Date* | Fecha de la transacción; puede tener formato incorrecto. | 2023-01-01 |

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

## 🛠Uso propuesto del Dataset
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
