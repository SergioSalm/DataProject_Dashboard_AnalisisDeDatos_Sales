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
Creamos una subcarpeta nueva dentro de 'Data' con el nombre '3-Data_analisis'. Dentro copiamos la excel car_Sales_transformados y la renombramos a car_sales_analisis_descriptivo.   
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


# Análisis descriptivo de las numéricas con las ventas
En la carpeta Data_analisis, duplicamos la excel 'car_sales_analisis_descriptivo' y la nombramos 'analisis_descriptivo_numericas_ventas'.  
Sobra la excel nueva, eliminamos la hoja 'analisis_descriptivo_categorica' y 'analisis_descriptivo_fechas'. Creamos la hoja 'analisis_ventas_numericas'.  
Realizamos el análisis de las columnas numéricas con las ventas de coches a través de tablas y gráficos.
Anual Income.  
Price

# Análisis descriptivo de las categoricas y temporales con las ventas
En la carpeta Data_analisis, duplicamos la excel 'car_sales_analisis_descriptivo' y la nombramos 'analisis_descriptivo_cat_temp_ventas'.  
Eliminamos la hoja 'analisis_descriptivo_numericas'. Creamos la hoja 'vista_categoricas' y 'vista_fechas'.
Creamos una columna nueva 'Annual income type' para agrupar los tipos de ingresos en 'Annual income type' en función del valor de la mediana de la columna Annual Income. Si los ingresos son iguales o inferiores a 100.000, el valor será 'Low'. Si los ingreos están entre 101.001 y 735.000 (el dobre de la mediana), el valor será 'High'. Y si están por encima de 1.470.001, el valor será 'Superior'. 
Cogemos el valor de 100.000 ya que el salario medio anual en estados unidos ronda los 77.000$. El siguiente rango de ingresos lo establecemos en 734.000$ ya que es la mediana de la columna 'Annual income'.
Realizamos el análisis de las columnas categoricas con las ventas de coches a través de tablas y gráficos dinámicos.
Gender.  
Color.  
Body style.  
Annual income type.  
Company.
Date.   
