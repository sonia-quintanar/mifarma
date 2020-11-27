![logo](https://github.com/sonia-quintanar/mifarma/blob/main/Im%C3%A1genes%20Home/logo.png)

# Descripción del proyecto

En este proyecto vamos a realizar un análisis de los productos que aparecen en la página principal, la presentación se realizará utilizando GIT.

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


Analizaremos cuáles son los productos que pertenecen a estas secciones, así como su marca, categoría, precio con descuento y sin descuento.

El objetivo final es observar si los productos que aparecen en esta página promocionados corresponden con la estrategia de marketing y ventas que tiene la empresa en mente.

Este método también puede servir para estudiar a la competencia, averiguando cuáles son los productos que  están promocionando, sus precios y estrategias. 

Con estos datos Mifarma podrá tomar decisiones para para garantizar a sus clientes el precio más bajo de cada producto y una amplica gama de productos demandados por los clientes.


## Pasos a seguir para el desarrollo del proyecto:


**1. Web scraping:**

Obtenemos los datos de la página web para realizar el análisis y demostración de la experiencia del uso de herramientas. 

Utilizamos Python para la obtención y manipulación de datos y después descargamos en formato CSV lo datos obtenidos. 

Indicamos los enlaces para consultarlo tanto en Jupyter Notebook:

 **- Categorías -**

![menú](https://github.com/sonia-quintanar/mifarma/blob/main/Home/men%C3%BA%20python.png)


- Jupyter Notebook:

https://github.com/sonia-quintanar/mifarma/blob/main/Home/Men%C3%BA%20-%20Submen%C3%BA.ipynb




**- Productos y marcas -**

![productos secciones](https://github.com/sonia-quintanar/mifarma/blob/main/Home/productos%20por%20secciones.png)


![productos](https://github.com/sonia-quintanar/mifarma/blob/main/Home/productos.png)


   - Jupyter Notebook:

https://github.com/sonia-quintanar/mifarma/blob/main/Home/Home.ipynb




**Por otro lado, se realiza la obtención de todas las marcas que vende Mifarma en su página web.**

![marcas excel](https://github.com/sonia-quintanar/mifarma/blob/main/Home/marcas%20excel.png)



   - Excel:

https://docs.google.com/spreadsheets/d/1PJS1idVMDd9y4txOev9ziN-kRLyCJ2fgMVgIz0numsw/edit?usp=sharing

   - Jupyter Notebook:

https://github.com/sonia-quintanar/mifarma/blob/main/Marcas/Marcas.ipynb






**2. Excel:**

Realizamos la manipulación y tratamiento de datos de los CSV descargados anteriormente.

https://docs.google.com/spreadsheets/d/1jIwqrgF0mtsyhZKxfmPhARh7CNM3u_CkAb42c6oLqd8/edit?usp=sharing

![dashboard](https://github.com/sonia-quintanar/mifarma/blob/main/Home/dashboard%20excel.png)



**En este documento nos encontramos con 4 hojas:**

 **- Dashboard:** conjunto de todos los datos obtenidos.

 **- Productos Home:** aparecen los productos que aparecen en la página principal separados por las tres secciones mencionadas anteriormente. 
 
 Podremos ver también el precio (con descuento y sin descuento), además del porcentaje del descuento aplicado que no aparece visible en la página web, y el promedio de descuentos por secciones.

 **- Marcas Home:** aparacen las marcas de los productos.

 **- Menú Home:** aparecen las categorías del menú.

Las operaciones que se han realizado nos servirán más adelante para realizar búsquedas en una base de datos con MySQL y visualización de datos con Tableau.




**3. Creación de base de datos con MySQL:**

Otra opción es generar una base de datos con MySQL con distintas tablas para realizar operaciones de consulta con los datos obtenidos anteriormente con Python.

Este es un ejemplo de la creación de la tabla "Novedades" y su contenido:

![Novedad1](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/Novedad1.png)
![Novedad2](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/Novedad2.png)
![Novedad3](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/Novedad3.png)




*Realizamos búsquedas de datos en MySQL con distintos filtros de ejemplo:*

   - Ordenar Top Ventas de mayor a menor precio:

![Top_ventas](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/Top%20Ventas%20-%20Odenar%20por%20precio%20desc%20sin%20dto.png)

   - Seleccionar los productos de la marca Santiveri de la tabla No te lo puedes perder...

![No_te_lo_puedes_perder](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/No%20te%20lo%20puedes%20perder%20-%20seleccionar%20productos%20marca%20Santiveri.png)


   - Seleccionar los productos con un precio de venta mayor de 10 € que pertenezcan a la categoría "Higiene y Salud" o a la categoría "Cosmética y Belleza".

![Novedad](https://github.com/sonia-quintanar/mifarma/blob/main/MySQL/Novedad.png)


**4. Tableau:**

Finalmente, procedemos con la parte de visualización de datos. Se puede acceder a través de este enlace:

https://public.tableau.com/profile/sonia7870#!/


**Comentarios**

![Categorías](https://github.com/sonia-quintanar/mifarma/blob/main/Tableau/Categor%C3%ADas.png)


Observamos que las categorías que más presencia tienen en la página principal son Cosmética y Belleza, Herbolario, Infantil e Higiene y Salud en ese mismo orden, el resto de categorías no tienen presencia.

![Marcas](https://github.com/sonia-quintanar/mifarma/blob/main/Tableau/Marcas.png)

Las marcas que aparecen en la página principal son las que vemos a continuación, siendo Santiveri, Nuxe y Binature las que más presencia tienen.

![Productos](https://github.com/sonia-quintanar/mifarma/blob/main/Tableau/Productos.png)

Podemos observar el precio de todos los productos de las tres secciones ordenados por orden alfabético viendo la relación de precios con y sin descuento y el porcentaje de descuento aplicado a cada producto.




**¿Corresponden los datos analizados anteriormente con la estrategia de marketing y ventas deseada de Mifarma?**

**Objetivo:** 

Garantizar a los clientes el precio más bajo del mercado de todos los productos ofertados, ajustando los precios, reduciendo costes, realizando un estudio exhaustivo y optimizando los recursos de Mifarma. 


