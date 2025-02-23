# Análisis de las ventas de coches

Vamos a realizar el estudio sobre las tendencias de ventas de coches en los años 2022 a 2023.
Descargamos el fichero desde la URL https://www.kaggle.com/datasets/safaeahb/car-sales-analysis-dashboard?select=car+sales.csv

En la primera parte del proyecto, una vez descargado el fichero en formato csv, los transformamos a excel en formato tabla para poder comenzar a trabajar con los datos.
Creamos la carpeta 'Data' que contendrá todos los ficheros. Dentro creamos la carpeta '1-Data_raw' con dos subcarpetas más. La primea es la carpeta csv con el fichero original descargado, y la segunda excel, con el fichero csv importado en excel en formato tabla. Al pasar al formato tabla, corregimos el valor de columna Engine 'DoubleÂ' por 'Double'.
Subimos el proyecto a Git.  

EL siguiente paso que realizamos es el estudio de las columnas, indicando una descripción de cada columna y analizando que columnas son relevantes para el análisis.  
Luego realizamos la transformación y limpieza.  

# Transformación y limpieza
Creamos una subcarpeta nueva dentro de 'Data' con el nombre '2-Datos_transformados'. Dentro creamos una nueva hoja excel a partir de la anterior y la renombramos a 'car_sales_transformados'.  

Creamos una columna nueva llamada 'Duplicados' para ver si tenemos algún identificador de ventas duplicado. No existen duplicados.

## Limpiamos los datos de la tabla

### Eliminamos datos irrelevantes
Eliminamos las columnas customer_name, dealer_no, phone

### Los tipos de datos correctos
Creamos una hoja nueva llamada 'Nulos' para ver cuantas columnas tienen valores nulos. Todos los datos están rellenos.
Vemos que todos los datos son correctos.

### Normalizar los datos
Todas las columnas tienen los datos normalizados

# Análisis descriptivo de columnas numéricas
Creamos una subcarpeta nueva dentro de 'Data' con el nombre '3-Data_analisis'. Dentro copiamos la excel car_Sales_transformados y la renombreamos a car_sales_analisis_descriptivo.   
Creamos una nueva hoja excel llamada 'analisis_descriptivo_numericas'  
Borramos la hoja Nulos.  
Eliminamos la columna 'Duplicado' de la hoja car_sales.  

Hemos analizado las estadísticas descriptivas para las siguientes columnas numéricas:  

Annual Income.
Price ($).

# Análisis descriptivo de columnas categoricas
Sobre la misma hoja excel anterior, creamos una hoja nueva llamada 'analisis_descriptivo_categorica' y analizamos las siguientes columnas categoricas:  
Gender.
Dealer_Name.
Company.
Model.
Engine. 
Transmission.
Color.
Body Style.
Dealer_Region.

# Análisis descriptivo de columnas fechas
Sobre la misma hoja excel anterior, creamos una hoja nueva llamada 'analisis_descriptivo_fechas' y analizamos las columnas de tipo fecha:  
Date
