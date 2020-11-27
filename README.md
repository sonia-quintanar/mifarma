![logo] (https://github.com/sonia-quintanar/mifarma/blob/main/Im%C3%A1genes%20Home/logo.png)

# Descripción del proyecto

En este proyecto, realizamos un análisis de los productos que aparecen en la página principal. 

El objetivo es verificar qué productos son los que queremos promocionar colocándolos estratégicamente para que el cliente sea lo primero que vea al entrar en la página web https://www.mifarma.es/.

Nos centraremos en las 3 secciones que aparecen:

- Top ventas
- No te puedes perder ...
- Novedad

Analizaremos cuáles son los productos que pertenecen a estas secciones, así como su marca, apartado del menú principal al que pertenecen, precio con y sin descuento. 

El objetivo final es observar si los productos que aparecen en esta página promocionados corresponden con la estrategia de márketing y ventas que tiene la empresa en mente.

Este método también puede servir para estudiar a la competencia, averiguando cuáles son los productos que  están promocionando, sus precios y estrategias. 

Con estos datos mifarma podrá tomar decisiones para para garantizar a sus clientes el precio más bajo de cada producto y una amplica gama de productos demandados por los clientes.


## Pasos a seguir para el desarrollo del proyecto:

1. **Web scrapping:

Obtener datos de la página web para realizar el análisis y demostración de la experiencia del uso de herramientas. 

Utilizo Python para la obtención y manipulación de datos. Después descargo en formato CSV lo datos obtenidos. 

Los enlaces tanto para consultar en Jupyter notebook o PDF son los siguientes:

**Menú

Jupyter Notebook:
https://github.com/sonia-quintanar/mifarma/blob/main/Home/Men%C3%BA%20-%20Submen%C3%BA.ipynb

PDF:
https://github.com/sonia-quintanar/mifarma/blob/main/Home/Men%C3%BA%20-%20Submen%C3%BA.pdf


**Productos y marcas

Jupyter Notebook:
https://github.com/sonia-quintanar/mifarma/blob/main/Home/Home.ipynb

PDF:
https://github.com/sonia-quintanar/mifarma/blob/main/Home/Home.pdf

También se realiza la obtención de todas las marcas que vende mifarma en su página web:

Jupyter Notebook:
https://github.com/sonia-quintanar/mifarma/blob/main/Marcas/Marcas.ipynb

PDF:
https://github.com/sonia-quintanar/mifarma/blob/main/Marcas/Marcas.pdf

Excel:
https://docs.google.com/spreadsheets/d/1PJS1idVMDd9y4txOev9ziN-kRLyCJ2fgMVgIz0numsw/edit?usp=sharing

2. **Excel:

Realizamos la manipulación y tratamiento de datos de los CSV descargados anteriormente.

https://docs.google.com/spreadsheets/d/1jIwqrgF0mtsyhZKxfmPhARh7CNM3u_CkAb42c6oLqd8/edit?usp=sharing

Nos encontramos con 4 hojas:

 - Dashboard: conjunto de todos los datos obtenidos.

 - Productos Home: aparecen los productos que aparecen en la página principal separados por las tres secciones mencionadas anteriormente. Podremos ver también el precio (con descuento y sin descuento), además del porcentaje del descuento aplicado que no aparece visible en la página web.

 - Marcas Home: aparacen las marcas de los productos.

 - Menú Home: aparecen las categorías del menú.

Las operaciones que se han realizado nos servirán más adelante para realizar búsquedas en una base de datos con MySQL y visualización de datos con Tableau.


3. **Creación de base de datos con MySQL:

Otra opción distinta a excel, es generar una base de datos con distintas tablas para realizar operaciones de consulta con los datos obtenidos anteriormente con Python.



4. Búsqueda de datos en MySQL para analizar hipótesis.

5. Tableau:

—> Contar cómo se ha hecho todo (capturas)
—> Gráficos de los resultados (búsquedas MySQL)
—> Pregunta: ¿Corresponden estos datos con la estrategia de marketing y ventas de mifarma?
—> Propuestas/Objetivos: Garantizar el precio más bajo del mercado de todos los productos (crear un boot para obtener los precios de los productos de las competencia y asegurarnos que es el precio más bajo.