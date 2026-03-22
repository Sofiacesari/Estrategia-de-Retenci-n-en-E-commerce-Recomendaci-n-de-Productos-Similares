**Estrategia de Retención en E-commerce: Recomendación de Productos Similares**

**Descripción**

Sistema de recomendación en moda que responde a uno de los puntos más críticos del e-commerce: el out of stock.
En lugar de cortar la experiencia, propone alternativas que preservan la lógica visual del producto original, tipo de prenda, color y estampa, sosteniendo la navegación y la intención de compra.

**Idea**

Cuando un producto no está disponible, no es solo un problema de stock, es una ruptura en la experiencia.
Este proyecto trabaja sobre ese momento: reemplazar la ausencia por continuidad.

**Dataset**

El modelo se construye a partir del dataset público de H&M Personalized Fashion Recommendations:
https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data

Un catálogo estructurado donde cada prenda puede leerse como un conjunto de atributos visuales y funcionales.

**Enfoque**
Cada producto se traduce a un espacio de características.
La similitud no es abstracta: se construye desde lo visible.

Se toman como base:

Tipo de prenda
Color
Apariencia gráfica (liso, estampado, etc.)

A partir de esto, el sistema encuentra las prendas más cercanas y las propone como sustitutos.

**Modelo**

Se implementa un modelo de K-Nearest Neighbors (KNN), que permite:

Medir proximidad entre productos
Ajustar la cantidad de alternativas (k)
Mantener coherencia entre el original y sus reemplazos

La lógica es simple: cercanía en datos → cercanía en percepción.

**Proceso**

Se trabajó sobre:

Validación y limpieza de datos
Análisis exploratorio del catálogo
Selección de variables relevantes
Construcción del modelo de similitud

El dataset presenta alta consistencia, lo que permitió enfocarse directamente en la lógica del sistema.

**Resultado**

Un sistema que:

Reemplaza productos agotados por alternativas coherentes
Evita la ruptura en la navegación
Convierte un punto de fricción en una oportunidad

**Stack**
Python · Pandas · Scikit-learn · Matplotlib · Seaborn
