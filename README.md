![logo](https://github.com/sonia-quintanar/mifarma/blob/main/Im%C3%A1genes%20Home/logo.png)

# Descripción del proyecto

En este proyecto vamos a realizar un análisis de los productos que aparecen en la página principal. 

El objetivo es verificar qué productos son los que queremos promocionar colocándolos estratégicamente para que el cliente sea lo primero que vea al entrar en la página web https://www.mifarma.es/.


**Las categorías que tenemos son:**

![Categorías](https://github.com/sonia-quintanar/mifarma/blob/main/Im%C3%A1genes%20Home/Men%C3%BA.png)


**Nos centraremos en las 3 secciones que aparecen:**


- Top ventas

![Top Ventas Home](https://github.com/sonia-quintanar/mifarma/blob/main/Im%C3%A1genes%20Home/Top%20Ventas.png)

- No te puedes perder ...

![No te lo puedes perder](https://github.com/sonia-quintanar/mifarma/blob/main/Im%C3%A1genes%20Home/No%20te%20puedes%20perder.png)

- Novedad

![Novedad](https://github.com/sonia-quintanar/mifarma/blob/main/Im%C3%A1genes%20Home/Novedad.png)


Analizaremos cuáles son los productos que pertenecen a estas secciones, así como su marca, apartado del menú principal al que pertenecen, precio con y sin descuento. 

El objetivo final es observar si los productos que aparecen en esta página promocionados corresponden con la estrategia de márketing y ventas que tiene la empresa en mente.

Este método también puede servir para estudiar a la competencia, averiguando cuáles son los productos que  están promocionando, sus precios y estrategias. 

Con estos datos mifarma podrá tomar decisiones para para garantizar a sus clientes el precio más bajo de cada producto y una amplica gama de productos demandados por los clientes.


## Pasos a seguir para el desarrollo del proyecto:


**1. Web scrapping:**

Obtener datos de la página web para realizar el análisis y demostración de la experiencia del uso de herramientas. 

Utilizo Python para la obtención y manipulación de datos. Después descargo en formato CSV lo datos obtenidos. 

Indico los enlaces para consultarlo tanto en Jupyter Notebook como en PDF:

 **- Menú -**

![menú](https://github.com/sonia-quintanar/mifarma/blob/main/Home/men%C3%BA%20python.png)


- Jupyter Notebook:

https://github.com/sonia-quintanar/mifarma/blob/main/Home/Men%C3%BA%20-%20Submen%C3%BA.ipynb

- PDF:

https://github.com/sonia-quintanar/mifarma/blob/main/Home/Men%C3%BA%20-%20Submen%C3%BA.pdf




**- Productos y marcas -**

![productos secciones](https://github.com/sonia-quintanar/mifarma/blob/main/Home/productos%20por%20secciones.png)


![productos](https://github.com/sonia-quintanar/mifarma/blob/main/Home/productos.png)


   - Jupyter Notebook:

https://github.com/sonia-quintanar/mifarma/blob/main/Home/Home.ipynb

   - PDF:

https://github.com/sonia-quintanar/mifarma/blob/main/Home/Home.pdf



**Por otro lado, se realiza la obtención de todas las marcas que vende mifarma en su página web.**

![marcas excel](https://github.com/sonia-quintanar/mifarma/blob/main/Home/marcas%20excel.png)



   - Excel:

https://docs.google.com/spreadsheets/d/1PJS1idVMDd9y4txOev9ziN-kRLyCJ2fgMVgIz0numsw/edit?usp=sharing

   - Jupyter Notebook:

https://github.com/sonia-quintanar/mifarma/blob/main/Marcas/Marcas.ipynb

   - PDF:

https://github.com/sonia-quintanar/mifarma/blob/main/Marcas/Marcas.pdf





**2. Excel:**

Realizamos la manipulación y tratamiento de datos de los CSV descargados anteriormente.

https://docs.google.com/spreadsheets/d/1jIwqrgF0mtsyhZKxfmPhARh7CNM3u_CkAb42c6oLqd8/edit?usp=sharing

![dashboard](https://github.com/sonia-quintanar/mifarma/blob/main/Home/dashboard%20excel.png)



**Nos encontramos con 4 hojas:**

 **- Dashboard:** conjunto de todos los datos obtenidos.

 **- Productos Home:** aparecen los productos que aparecen en la página principal separados por las tres secciones mencionadas anteriormente. Podremos ver también el precio (con descuento y sin descuento), además del porcentaje del descuento aplicado que no aparece visible en la página web.

 **- Marcas Home:** aparacen las marcas de los productos.

 **- Menú Home:** aparecen las categorías del menú.

Las operaciones que se han realizado nos servirán más adelante para realizar búsquedas en una base de datos con MySQL y visualización de datos con Tableau.




**3. Creación de base de datos con MySQL:**

Otra opción distinta a excel, es generar una base de datos con distintas tablas para realizar operaciones de consulta con los datos obtenidos anteriormente con Python.

*Búsqueda de datos en MySQL con distintos filtros de ejemplo:*

   - Ordenar Top Ventas por precio de mayor a menor:*

![Top_ventas](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/Top%20Ventas%20-%20Odenar%20por%20precio%20desc%20sin%20dto.png)

   - Seleccionar los productos de la marca Santiveri de la tabla No te lo puedes perder...*

![No_te_lo_puedes_perder](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/No%20te%20lo%20puedes%20perder%20-%20seleccionar%20productos%20marca%20Santiveri.png)


   - Seleccionar los productos con un precio de venta mayor de 10 € que pertenezcan a la categoría "Higiene y Salud" o a la categoría "Cosmética y Belleza".*

![Novedad](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/Novedad.png)


5. Tableau:

—> Contar cómo se ha hecho todo (capturas)
—> Gráficos de los resultados (búsquedas MySQL)
—> Pregunta: ¿Corresponden estos datos con la estrategia de marketing y ventas de mifarma?
—> Propuestas/Objetivos: Garantizar el precio más bajo del mercado de todos los productos (crear un boot para obtener los precios de los productos de las competencia y asegurarnos que es el precio más bajo.