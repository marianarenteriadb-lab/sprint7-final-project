ConnectaTel: Análisis de Clientes y Patrones de Uso
Objetivo del Proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel a partir de información demográfica y registros de uso de servicios de telecomunicaciones. Mediante técnicas de limpieza, exploración y segmentación de datos, se busca identificar patrones de consumo, detectar valores atípicos y generar recomendaciones que apoyen la toma de decisiones del negocio.

Datasets Utilizados

El proyecto utiliza dos conjuntos de datos principales:

users

Contiene información demográfica y de registro de los usuarios:

user_id
first_name
last_name
age
city
reg_date
plan
churn_date
usage

Contiene los registros de uso de los servicios de telecomunicaciones:

id
user_id
type (call o text)
date
duration
length
Etapas del Análisis
1. Exploración inicial de datos
Revisión de estructura y tipos de datos.
Identificación de valores faltantes y posibles inconsistencias.
2. Limpieza y preparación de datos
Conversión de variables de fecha.
Corrección de valores centinela.
Tratamiento de fechas fuera de rango.
Estandarización de variables categóricas.
Análisis de valores faltantes.
3. Análisis exploratorio de datos (EDA)
Estadísticas descriptivas.
Distribuciones de variables numéricas.
Comparación de patrones de uso por plan.
4. Detección de Outliers
Visualización mediante boxplots.
Cálculo de límites utilizando el método IQR.
Evaluación de impacto de valores atípicos.
5. Segmentación de Clientes
Segmentación por nivel de uso.
Segmentación por grupos de edad.
Análisis comparativo entre segmentos.
6. Generación de Insights
Identificación de patrones relevantes para el negocio.
Elaboración de recomendaciones comerciales.
Cómo Ejecutar el Proyecto
Opción 1: Google Colab
Descarga el archivo .ipynb.
Ingresa a Google Colab.
Selecciona Archivo → Subir cuaderno.
Carga el notebook.
Ejecuta las celdas en orden.
Opción 2: Jupyter Notebook
Clona el repositorio:
git clone https://github.com/marianarenteriadb-lab/sprint7-final-project.git
Instala las dependencias:
pip install pandas numpy matplotlib seaborn
Abre Jupyter Notebook.
Ejecuta el archivo:
jupyter notebook
Guía de Reproducción

Para reproducir completamente el análisis:

Cargar los datasets originales.
Ejecutar las celdas de limpieza y transformación.
Ejecutar las secciones de análisis exploratorio.
Ejecutar la detección de outliers.
Ejecutar la segmentación de clientes.
Revisar los insights y conclusiones finales.
Herramientas Utilizadas
Python
Pandas
NumPy
Matplotlib
Seaborn
Principales Hallazgos
Se identificaron registros con fechas fuera de rango que requirieron corrección.
Se detectaron usuarios con patrones de consumo significativamente superiores al promedio.
Se construyeron segmentos de clientes basados en edad y nivel de uso.
Los resultados permiten generar recomendaciones para optimizar la oferta de planes y estrategias de retención.
