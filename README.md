# Movie data analysis

Este proyecto consiste en el analisis de un dataset de películas, que incluyen: limpieza de datos y visualización de resultados.

## Contenido del repositorio
- `moviesdataset_clean.csv` → dataset limpio, listo para análisis.
- `MartinezL-movie_challenge-data.ipynb` → notebook con la limpieza, análisis y gráficos.

## Limpieza de datos
- Se eliminaron filas con valores nulos en columnas clave (`Genre`, `Budget`, `Revenue`, `IMDB_Rating`).
- Se convirtieron valores inconsistentes:
  - `"80M"` → `80000000`
  - `"Two Thousand"` → `2000`
- Se eliminaron filas duplicadas.
- Se creó la columna `Profit` = `Revenue - Budget`. Esta columna se creo para mostrar las ganancias netas, es decir la diferencia entre lo que se invirtio y lo que se recaudo en cada pelicula.

## Insights principales y visualizaciones
1. **Géneros más rentables:**
   
![Ganancia y Rating promedio por genero](ganancia_rating_por_genero.png)

Se observo que los generos mas rentables son en primer lugar drama y comedia, seguidos por gran diferencia por acción, fantasia y romance. El género que menos rentabilidad tiene es el de thriller, lo cual se puede deber a la inversión que se debe realizar para llevar a cabo cada pelicula (efectos especiales, maquillaje, escenografías, etc)

2. **Tendencia de rating por género:** 

![Tendencia de rating por géneros](rating_por_genero.png)

Los géneros que mejor promedio de puntuación de rating obtuvieron son: Acción, comedia, drama y thriller. Los géneros romance y fantasia obtuvieron un promedio de rating por debajo de 5.
   
3. **Relacion beneficio neto-rating por género:** 

![Evolución de ratings y ganancias por año](evolucion_ganancia_rating_por_anio.png)

Se puede observar que hay una tendencia a que cuando el rating promedio de los géneros son buenos, las ganancias de los mismos también lo han sido. Por ende, podemos establecer a primera vista una relacion directa entre ambos.
   
4. **Relación presupuesto–ingreso:** 

![Relación presupuesto vs recaudación por género](comparacion_inversionvsrecaudacion_por_genero.png)

Los géneros de comedia y drama, requieren una menor inversión para la recaudación obtenida en comparación con thriller y romance. Los géneros fantasia y acción generan ganancias pero la diferencia entre el presupuesto y la recaudación es mas pequeña.

## Conclusión
En el análisis realizado se puede observar patrones interesantes en los datos de películas, permitiendo identificar los géneros más rentables, la evolución de calificaciones y la relación entre inversión y ganancias.
Cabe destacar que la cantidad de datos era limitada, lo que puede afectar en algunas columnas la robustez de los resultados, por lo que los patrones que se observaron son indicativos.
Para analisis futuros, sería interesante incluir mayor cantidad de peliculas de generos variados, duración de las mismas, país de producción y paises o areas donde generaron mas recaudación, entre otros, para obtener conclusiones mas precisas.
