# Proyecto de Análisis de Datos

¡Bienvenido/a! Este repositorio ilustra un proceso integral de **Análisis de Datos** que inicia con un **Análisis Exploratorio (EDA)** y evoluciona hacia **Análisis Avanzados**, incluyendo reportes y visualizaciones. A continuación, encontrarás una descripción de cada fase y los pasos principales para reproducir este proyecto.

---

## Diagrama General del Flujo

Para representar las distintas etapas de nuestro análisis, utilizamos el siguiente diagrama:

![image](https://github.com/user-attachments/assets/622e7622-921b-457b-b8d6-f0bbc6b9a2a8)


> **Nota:** Asegúrate de colocar la imagen en la carpeta `docs` y renombrarla a `data_analysis_flow.png` o ajusta la ruta según tu organización de archivos.

Este flujo se divide en dos grandes fases:

1. **Exploratory Data Analysis (EDA)** (Pasos 1 al 9)  
2. **Advanced Analytics** (Pasos 10 al 12)

---

## 1. Exploratory Data Analysis (EDA)

En esta primera fase, se realiza un estudio preliminar de los datos para comprender su estructura, identificar patrones y detectar posibles inconsistencias.

### 1.1 Database Exploration
- **Objetivo**: Identificar la estructura y contenido de las tablas.
- **Actividad Clave**: Uso de `INFORMATION_SCHEMA.TABLES` y `INFORMATION_SCHEMA.COLUMNS` para listar tablas y campos, validando la calidad y consistencia de la información.

### 1.2 Dimensions Exploration
- **Objetivo**: Conocer en detalle las dimensiones (Clientes, Productos, etc.).
- **Actividad Clave**: Identificar valores únicos, clasificar campos relevantes y verificar integridad de la información (por ejemplo, países o categorías).

### 1.3 Data Exploration
- **Objetivo**: Explorar los registros y revisar datos atípicos o faltantes.
- **Actividad Clave**: Análisis de rangos de fechas, outliers y conteos de registros para asegurar datos consistentes.

### 1.4 Measures Exploration (Big Numbers)
- **Objetivo**: Calcular métricas globales que den un panorama general (ventas totales, número de clientes, etc.).
- **Actividad Clave**: Uso de funciones de agregación (`SUM`, `COUNT`, `AVG`) para obtener indicadores clave del negocio.

### 1.5 Magnitude Analysis
- **Objetivo**: Evaluar la escala de los datos en dimensiones o categorías específicas.
- **Actividad Clave**: Sumar ventas o clientes por categoría, país, línea de producto, etc.

### 1.6 Ranking (Top N / Bottom N)
- **Objetivo**: Ordenar productos, clientes u otras entidades según su rendimiento.
- **Actividad Clave**: Uso de funciones de ventana (`RANK`, `DENSE_RANK`) o consultas `TOP` para encontrar los más y menos destacados.

### 1.7 Reporting
- **Objetivo**: Consolidar los resultados en reportes o vistas analíticas.
- **Actividad Clave**: Creación de vistas (por ejemplo, `report_customers`, `report_products`) que presenten métricas clave de forma amigable.

### 1.8 Data Segmentation
- **Objetivo**: Clasificar datos en grupos (segmentos) con base en criterios de negocio (por ejemplo, gasto total o antigüedad).
- **Actividad Clave**: Uso de `CASE WHEN` para categorizar clientes como VIP, Regulares o Nuevos.

### 1.9 Part-to-Whole Analysis
- **Objetivo**: Medir la contribución de cada categoría al total (por ejemplo, porcentaje de ventas por producto).
- **Actividad Clave**: Uso de `SUM(...) OVER()` para calcular porcentajes sobre la suma global.

---

## 2. Advanced Analytics

Una vez comprendidos los datos, pasamos a técnicas más especializadas para descubrir tendencias y medir rendimientos en el tiempo.

### 2.1 Performance Analysis
- **Objetivo**: Comparar métricas actuales con periodos anteriores y medir la evolución del negocio.
- **Actividad Clave**: Funciones de ventana como `LAG` o `LEAD` para comparar ventas año contra año, o mes contra mes.

### 2.2 Cumulative Analysis
- **Objetivo**: Obtener totales y promedios acumulados, fundamentales para detectar tendencias de crecimiento o declive.
- **Actividad Clave**: Uso de `SUM() OVER(ORDER BY fecha)` y cálculos de promedio móvil para observar la evolución de métricas clave.

### 2.3 Change-Over-Time (Trends)
- **Objetivo**: Visualizar y entender cómo varían las métricas a lo largo de periodos específicos (mes, trimestre, año).
- **Actividad Clave**: Agrupaciones por intervalos de tiempo (`DATETRUNC`, `FORMAT`, etc.) para analizar picos y estacionalidad.

---




