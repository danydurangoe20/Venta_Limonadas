# 🍋 Análisis Exploratorio y Predicción de Ventas - Lemonade Dataset

## 📌 Descripción del Proyecto

Este proyecto desarrolla un análisis exploratorio de datos (EDA) y un modelo de regresión lineal utilizando Python sobre un conjunto de datos de ventas de limonada.

El objetivo principal es comprender cómo variables como la temperatura, las precipitaciones y la cantidad de volantes distribuidos afectan las ventas diarias, además de construir un modelo predictivo capaz de estimar las ventas.

---

# 📂 Contenido del Proyecto

* Carga y exploración de datos
* Limpieza y transformación de variables
* Estadística descriptiva
* Medidas de tendencia central
* Medidas de dispersión
* Detección de valores atípicos (Outliers)
* Análisis de asimetría y curtosis
* Visualización de datos
* Matriz de correlación
* Análisis de relaciones entre variables
* Modelo de regresión lineal
* Evaluación del modelo predictivo

---

# 🛠️ Tecnologías Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

# 📊 Variables Analizadas

| Variable    | Descripción                       |
| ----------- | --------------------------------- |
| Date        | Fecha del registro                |
| Día         | Día de la semana                  |
| Temperature | Temperatura diaria                |
| Rainfall    | Nivel de precipitaciones          |
| Flyers      | Cantidad de volantes distribuidos |
| Price       | Precio del producto               |
| Sales       | Ventas realizadas                 |

---

# 🔍 Análisis Exploratorio de Datos

Durante el análisis se realizaron:

## ✅ Conversión de Temperatura

La temperatura originalmente se encontraba en grados Fahrenheit, por lo que se convirtió a grados Celsius utilizando:

```python
df['Temperature'] = (df['Temperature'] - 32) * 5 / 9
```

---

## ✅ Estadística Descriptiva

Se calcularon:

* Media
* Mediana
* Moda
* Cuartiles
* Desviación estándar
* Varianza
* Rango

---

## ✅ Detección de Outliers

Se utilizó el método del rango intercuartílico (IQR) para identificar valores atípicos en las variables numéricas.

---

## ✅ Visualizaciones Generadas

* Histogramas
* Boxplots
* Heatmap de correlación
* Gráficos de dispersión
* Evolución temporal de ventas
* Promedio de ventas por día

---

# 📈 Modelo Predictivo

Se implementó un modelo de regresión lineal para predecir las ventas (`Sales`) usando:

* Temperatura
* Precipitaciones
* Volantes

## Variables Predictoras

```python
X = df[['Temperature', 'Rainfall', 'Flyers']]
```

## Variable Objetivo

```python
y = df['Sales']
```

---

# 🤖 Resultados del Modelo

## Métricas obtenidas

| Métrica | Resultado |
| ------- | --------- |
| MAE     | 1.52      |
| MSE     | 5.46      |
| RMSE    | 2.34      |
| R²      | 0.89      |

El modelo logró explicar aproximadamente el **89% de la variabilidad de las ventas**, mostrando un desempeño bastante sólido.

---

# 📷 Ejemplos de Gráficas

El proyecto incluye visualizaciones como:

* Ventas semanales
* Distribución de variables
* Correlaciones
* Predicciones vs valores reales

---

# ▶️ Cómo Ejecutar el Proyecto

## 1. Clonar el repositorio

```bash
git clone https://github.com/tuusuario/nombre-repositorio.git
```

## 2. Instalar dependencias

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 3. Ejecutar el notebook o script

```bash
python main.py
```

o abrir el notebook en Jupyter/Google Colab.

---

# 📚 Aprendizajes Obtenidos

Este proyecto permitió aplicar conceptos de:

* Ciencia de datos
* Estadística descriptiva
* Visualización de datos
* Machine Learning
* Regresión lineal
* Evaluación de modelos predictivos

---

# 👨‍💻 Autor

Proyecto desarrollado por **Dany Durango Escobar**.

---

# ⭐ Contribuciones

Las contribuciones, sugerencias y mejoras son bienvenidas.

---
