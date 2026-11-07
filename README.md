# Análisis Geoespacial de Microbasurales Urbanos en San Miguel de Tucumán

Pipeline ETL y análisis de proximidad espacial a gran escala para modelar la distribución y correlación territorial de 242 microbasurales sobre más de 157.000 parcelas catastrales en San Miguel de Tucumán.

---

## 🎯 Objetivo del Proyecto

Modelar los patrones de concentración de residuos a cielo abierto en el tejido urbano para identificar corredores críticos de vulnerabilidad ambiental y optimizar las rutas de recolección y fiscalización municipal.

---

## 📊 Principales Hallazgos y Métricas

* **Escala del Análisis:** Procesamiento de **157.000+ parcelas catastrales** y **242 puntos georreferenciados de microbasurales**.
* **Corredores Críticos:** El **30,17% de los basurales** se concentran en zonas de amortiguamiento (*buffers*) directas a corredores viales principales y trazas ferroviarias.
* **Patrón de Proximidad:** Mediante *Spatial Joins* y análisis de vecinos más cercanos (*Nearest Neighbor*), se identificaron clústeres donde la recurrencia de acumulación de residuos se vincula con vacíos urbanos e infraestructura de conectividad interjurisdiccional.

---

## 🛠️ Stack Tecnológico

* **Lenguaje:** `Python`
* **Librerías Geoespaciales:** `GeoPandas`, `Shapely`, `PyProj` (sistemas de coordenadas CRS / UTM)
* **ETL & Data Wrangling:** `Pandas`, `NumPy`, Web Scraping / APIs para integración de capas
* **Visualización Geoespacial:** `Folium` (mapas de calor y coropletas interactivas)

---

## 🔬 Metodología Aplicada

1. **Extracción y Limpieza:** Normalización de capas vectoriales catastrales y geolocalización de reportes de microbasurales.
2. **Transformación de Coordenadas:** Reproyección al sistema métrico local (UTM / Gauss-Krüger) para garantizar mediciones de distancia y superficie euclidianas precisas.
3. **Análisis de Buffers y Proximidad:** Construcción de áreas de influencia (*buffers* concéntricos) sobre vías primarias y cálculo de intersecciones espaciales.
4. **Visualización y Reporte:** Renderizado de capas geoespaciales dinámicas con marcadores segmentados por severidad.

---

## 📁 Estructura del Proyecto

* `notebooks/`: Jupyter Notebook con el pipeline ETL, análisis espacial y cálculo de métricas.
* `maps/`: Archivos exportados en formato HTML interactivo (`Folium`).
* `informes/`: resumen ejecutivo del trabajo.

---

## 👤 Autor

**Santiago Rodríguez Garay**  
*Lic. en Gestión Turística & Google Certified Advanced Data Analyst*  
* [LinkedIn](https://www.linkedin.com/in/santiago-rodriguez-garay-9b2a3034a)
* [Email](mailto:santiagomanuelrg@gmail.com)
