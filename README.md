# Predicción de Tickets Altos en una Ferretería

Proyecto de Data Science y Machine Learning orientado al análisis de ventas y predicción de tickets altos en una empresa del rubro ferretero.

## Objetivo del proyecto

El objetivo principal es identificar los factores que influyen en las ventas de alto valor y desarrollar un modelo predictivo capaz de anticipar qué operaciones tienen mayor probabilidad de convertirse en tickets altos.

A través de técnicas de análisis exploratorio de datos y Machine Learning, se busca transformar datos históricos en información accionable para mejorar la toma de decisiones comerciales.

---

# Problema de negocio

Las empresas comerciales generan grandes volúmenes de datos diariamente, pero muchas veces no logran aprovecharlos estratégicamente.

En este caso, el desafío consiste en detectar patrones asociados a ventas de alto valor para optimizar:

- promociones,
- campañas comerciales,
- medios de pago,
- estrategias operativas,
- y acciones orientadas a maximizar ingresos.

---

# Dataset

El dataset contiene información de ventas de una ferretería, incluyendo variables como:

- sucursal,
- provincia,
- categoría de producto,
- medio de pago,
- fecha y hora,
- promociones,
- comportamiento de compra,
- y monto de venta.

---

# Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Proceso realizado

## 1. Limpieza y transformación de datos

- tratamiento de valores faltantes,
- conversión de fechas,
- creación de variables temporales,
- encoding de variables categóricas.

## 2. Análisis Exploratorio de Datos (EDA)

Se analizaron patrones de comportamiento relacionados con:

- categorías con mayores ventas,
- tickets altos,
- medios de pago,
- horarios y días de compra,
- promociones.

## 3. Ingeniería de atributos

Se crearon variables contextuales como:

- mes,
- día de semana,
- horario,
- fin de semana,
- promociones activas,
- compra múltiple.

Además, se aplicó prevención de Data Leakage eliminando variables que contenían información directamente relacionada con el resultado final de la venta.

## 4. Modelado de Machine Learning

Se entrenaron distintos modelos predictivos para clasificación:

- Regresión Logística
- Random Forest

## 5. Validación y optimización

- train/test split
- validación cruzada
- GridSearchCV
- comparación de métricas

---

# Variable objetivo

Se construyó la variable:

```python
ticket_alto
donde:

1 = venta superior al percentil 75
0 = resto de las ventas

Esto permitió transformar el problema en una tarea de clasificación binaria.


Principales insights
El 25% de las ventas concentra los tickets más altos.
Algunas categorías presentan mayor probabilidad de generar ventas de alto valor.
Determinados horarios y días muestran mayor concentración de tickets altos.
El medio de pago influye en el comportamiento de compra.
Las promociones impactan positivamente en el valor de las ventas.
Resultados

El modelo desarrollado logró identificar patrones relevantes asociados a tickets altos y permitió anticipar operaciones de mayor valor utilizando únicamente variables conocidas antes de concretar la venta.

Esto demuestra el potencial del análisis predictivo como herramienta de apoyo para decisiones comerciales.

Estructura del repositorio
├── data/
├── notebooks/
├── images/
├── presentation/
├── README.md
Autora
Maria Eugenia Acosta

Proyecto desarrollado para la Diplomatura de Data Science & Machine Learning en Coderhouse.

Contacto

GitHub: Eugeacosta
