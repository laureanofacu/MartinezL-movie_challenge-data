# Movie data analysis

Este proyecto consiste en el analisis de un dataset de películas, que incluyen: limpieza de datos y visualización de resultados.

## Contenido del repositorio
- `moviesdataset_clean.csv` → dataset limpio, listo para análisis.
- `MartinezL-movie_challenge-data.ipynb` → notebook con la limpieza, análisis y gráficos.
- `README.md`

## Limpieza de datos
- Se eliminaron filas con valores nulos en columnas clave (`Genre`, `Budget`, `Revenue`, `IMDB_Rating`).
- Se convirtieron valores inconsistentes:
  - `"80M"` → `80000000`
  - `"Two Thousand"` → `2000`
- Se eliminaron filas duplicadas.
- Se creó la columna `Profit` = `Revenue - Budget`. Esta columna se creo para mostrar las ganancias netas, es decir la diferencia entre lo que se invirtio y lo que se recaudo en cada pelicula.

## Insights principales
1. **Géneros más rentables:**
2. **Tendencia de rating por año:**
3. **Relación presupuesto–ingreso:**

## Visualizaciones
1. **Ganancia promedio y rating promedio por género:**
2. **Distribución de ratings IMDB:**


## Conclusión
