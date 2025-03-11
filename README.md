# DataWarehouseAnalytics - EDA

Este proyecto implementa un Data Warehouse para realizar un Análisis Exploratorio de Datos (EDA) sobre ventas, clientes y productos. Los scripts SQL logran:

- **Creación y configuración de la base de datos:**  
  - Eliminación y recreación limpia de la base de datos `DataWarehouseAnalytics`.

- **Definición de esquemas y tablas:**  
  - Organización de la información en esquemas, con tablas de dimensiones (`dim_customers`, `dim_products`) y una tabla de hechos (`fact_sales`).

- **Carga masiva de datos:**  
  - Importación de datos desde archivos CSV usando `BULK INSERT`.

- **Consultas analíticas avanzadas:**  
  - Ejemplos de análisis de métricas clave, tendencias temporales, segmentación y ranking de productos y clientes.

- **Vistas consolidadas:**  
  - Creación de vistas (`report_customers` y `report_products`) que resumen y facilitan el análisis de los datos.

Este enfoque permite extraer insights valiosos y entender el rendimiento del negocio de forma clara y efectiva.
