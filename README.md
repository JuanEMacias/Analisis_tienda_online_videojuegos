<h1 align="center"> Análisis de datos para tienda online de videojuegos 🎮  </h1>

## Descripción
***
En este proyecto se trabaja para la tienda online ICE que vende videojuegos por todo el mundo. Las reseñas de usuarios y expertos, los géneros, las plataformas (por ejemplo, Xbox o PlayStation) y los datos históricos sobre las ventas de juegos están disponibles en fuentes abiertas. 
Para este caso, se deben identificar patrones que determinen si un juego tiene éxito o no. Esto te permitirá detectar proyectos prometedores y planificar campañas publicitarias.
Hay datos que se remontan a 2016. Estos datos se usan para la hipotética planeación de una campaña para 2017.
El dataset contiene una columna "rating" que almacena la clasificación ESRB de cada juego. El Entertainment Software Rating Board (la Junta de clasificación de software de entretenimiento) evalúa el contenido de un juego y asigna una clasificación de edad como Adolescente o Adulto.

## Descripción de los datos 

Los datos se encuentran en el  archivo /datasets/games.csv cuyas columnas son: 

— Name (Nombre)

— Platform (Plataforma)

— Year_of_Release (Año de lanzamiento)

— Genre (Género) 

— NA_sales (ventas en Norteamérica en millones de dólares estadounidenses) 

— EU_sales (ventas en Europa en millones de dólares estadounidenses) 

— JP_sales (ventas en Japón en millones de dólares estadounidenses) 

— Other_sales (ventas en otros países en millones de dólares estadounidenses) 

— Critic_Score (máximo de 100) 

— User_Score (máximo de 10) 

— Rating (ESRB)

![Muestra de los datos](https://github.com/user-attachments/assets/7e315e44-40dc-4335-940c-73341900406f)


## Tareas 

### 1. Preparación de los datos. 

Se reemplazan los nombres de las columnas y se convierten los datos en los tipos necesarios.

Tratarmos los valores ausentes.

Calculamos las ventas totales (la suma de las ventas en todas las regiones) para cada juego y colocando estos valores en una columna separada.

### 2. Análisis de los datos. 

* Observamos cuántos juegos fueron lanzados en diferentes años. ¿Son significativos los datos de cada período?
* Observamos cómo varían las ventas de una plataforma a otra. 
* Determinamos para qué período debemos tomar datos para trabajar solo con los datos que se consideran relevantes.
  
Contestamos las siguientes preguntas dentro del análisis:

* ¿Qué plataformas son líderes en ventas? 
* ¿Cuáles crecen y cuáles se reducen? Elige varias plataformas potencialmente rentables.
* ¿Son significativas las diferencias en las ventas? 
* Qué sucede con las ventas promedio en varias plataformas? 
* ¿Cuál es la correlación entre las reseñas y las ventas?
* ¿Qué se puede decir de los géneros más rentables? 
* ¿Podemos generalizar acerca de los géneros con ventas altas y bajas?
  
### 3. Creamos un perfil de usuario para cada región

Para cada región (Norteamérica, Europa y Japón) determinamos:

*	Las cinco plataformas principales. Describimos las variaciones en las cuotas de mercado de una región a otra.
*	Los cinco géneros principales. 
*	Si las clasificaciones de ESRB afectan a las ventas en regiones individuales.

### 4. Pruebas de hipótesis:

Se realizan pruebas estadísticas para probar las siguientes hipótesis:
* Las calificaciones promedio de los usuarios para las plataformas Xbox One y PC son las mismas.
*  Las calificaciones promedio de los usuarios para los géneros de Acción y Deportes son diferentes.


## Tecnologías
***
Los recursos utilizados en este proyecto son:
* Librerías de Python:
  * Pandas
  * Numpy
  * Matplotlib
  * Scipy stats
* Jupyter Notebooks

Las librerías pandas y numpy se utilzian principalmente en la preparación de los datos, para eliminar valores ausentes, duplicados o posibles valores atípicos; así como la agregación de columnas requridas.  
La librería Matplotib se usa para visuzalización de las estadísticas y la librería Scipy stats se susa para poder relaizar los cálculos de las pruebas de hipótesis. 

## Uso del código 
Todos los bloques de código se encuentran en el archivo .ipynb y el set de datos en el arhivo .csv.
Para utilizarlo descargar los archivos csv, copie el cuaderno y ejecutar los bloques de código.
