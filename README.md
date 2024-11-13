# PEC 2: Técnicas de Visualización de Datos

Este repositorio contiene el código y las visualizaciones desarrolladas para la PEC 2 de la asignatura de visualización de datos. En este proyecto, exploramos tres técnicas de visualización de datos: **cartogramas**, **mapas de flujo** y **gráficos de bala**, cada uno aplicado a datos de diferentes tipos para analizar sus características y casos de uso.

## Técnicas de Visualización

### 1. Cartograma
Un **cartograma** ajusta el tamaño de las regiones geográficas en función de una variable cuantitativa, como la población. En el código proporcionado, se utiliza un cartograma que representa el tamaño relativo de la población de varios países (EE. UU., India, Brasil, Rusia, España, Australia, México y Nigeria) mediante círculos proporcionalmente escalados.

- **Librerías**: `geopandas`, `matplotlib`, `pandas`
- **Datos**: Población aproximada en millones para cada país.
- **Archivo Shapefile**: `ne_110m_admin_0_countries.shp` de [Natural Earth Data](https://www.naturalearthdata.com/)

### 2. Mapa de Flujo
Un **mapa de flujo** visualiza movimientos entre ubicaciones, como rutas de migración o de comercio. Este tipo de visualización es útil para entender patrones de movimiento y conexiones.

### 3. Gráfico de Bala
El **gráfico de bala** permite comparar un valor actual con un objetivo dentro de un rango de rendimiento. Es especialmente útil en evaluaciones de desempeño, como en métricas de negocio o indicadores clave (KPIs).

## Estructura del Código

El código para cada visualización está contenido en archivos separados y organizados por técnica. A continuación, se describe el flujo general del código para el **cartograma** (la técnica central en este repositorio):

1. **Carga de Librerías**: Importa `geopandas`, `matplotlib` y `pandas` para el manejo de datos geoespaciales y visualización.
2. **Carga de Datos Geográficos**: Usa un archivo shapefile (`ne_110m_admin_0_countries.shp`) para obtener la geometría de los países.
3. **Integración de Datos de Población**: Se crea un `DataFrame` con datos de población y se fusiona con los datos geográficos.
4. **Creación de la Visualización**: Genera un cartograma en el que cada país aparece representado por un círculo proporcional a su población.
5. **Etiquetas y Personalización**: Añade etiquetas con los nombres de los países para facilitar la interpretación.

## Requisitos

- **Python 3.7+**
- **Librerías**:
  - `geopandas`
  - `matplotlib`
  - `pandas`

Para instalar las dependencias, puedes usar el siguiente comando:
```bash
pip install geopandas matplotlib pandas
