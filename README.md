# TelecomX LATAM - Analisis de Evasion de Clientes (Churn)

## Descripcion del Proyecto
Este proyecto de analisis de datos tiene como objetivo comprender y mitigar la evasion de clientes (Churn) en TelecomX LATAM, una empresa del sector de telecomunicaciones. A traves de un proceso integral de ETL (Extraccion, Transformacion y Carga) y Analisis Exploratorio de Datos (EDA), el proyecto identifica los factores clave que motivan a los usuarios a cancelar sus servicios, proporcionando insights accionables para la toma de decisiones estrategicas.

Este repositorio documenta todo el flujo de trabajo, desde el procesamiento de datos crudos anidados hasta la generacion de visualizaciones y conclusiones de negocio.

## Estructura y Caracteristicas Principales
El analisis se desarrolla mediante Python y abarca las siguientes fases:

1. Extraccion de Datos: Lectura de datos JSON desde repositorios externos, manejando estructuras anidadas complejas (diccionarios dentro de columnas).
2. Transformacion y Limpieza: 
   - Desanidado de variables clave (genero, tipo de contrato, metodos de pago).
   - Limpieza de datos nulos y estandarizacion de la variable objetivo (Evasion).
   - Ingenieria de caracteristicas (creacion de metricas derivadas como cargos diarios).
3. Analisis Exploratorio (EDA): Evaluacion estadistica y visual de patrones de comportamiento de los usuarios.
4. Informe de Negocio: Recomendaciones estrategicas para reducir la tasa de abandono basadas en evidencia.

## Visualizaciones Destacadas

A continuacion, se presentan algunos de los hallazgos visuales mas importantes del analisis exploratorio:

### Distribucion General de la Evasion
El analisis inicial revela la proporcion de clientes que han abandonado el servicio frente a los retenidos.

### Comportamiento segun Variables Categoricas
Se observa una fuerte correlacion entre la evasion y factores como el tipo de contrato (mensual vs. anual) y el servicio de internet (Fibra Optica).

### Impacto de las Variables Numericas
El analisis de distribucion muestra que el riesgo critico de abandono se concentra en los primeros meses de antiguedad y en los rangos de facturacion mas altos.

## Tecnologias Utilizadas
- Lenguaje: Python 3.11
- Entorno: Jupyter Notebook
- Manipulacion de Datos: Pandas
- Visualizacion de Datos: Matplotlib, Seaborn

## Requisitos Previos e Instalacion
Para ejecutar este proyecto de forma local, clona el repositorio e instala las dependencias:

1. Clona el repositorio:
   git clone https://github.com/gianpierreSO/AnalisisEvasion1/

2. Instala las librerias necesarias:
   pip install pandas matplotlib seaborn jupyter

3. Inicia el entorno:
   jupyter notebook

4. Ejecuta el archivo `TelecomX_LATAM.ipynb`.

## Resultados Clave
- La tasa historica de evasion es del 26.5%.
- Vulnerabilidad Temprana: Riesgo critico de abandono durante los primeros 6 meses de servicio.
- Flexibilidad Contractual: Los contratos "mes a mes" carecen de barreras de retencion efectivas.
- Perfil de Riesgo: Los usuarios de Fibra Optica con pagos mediante cheque electronico presentan la mayor propension a cancelar.
