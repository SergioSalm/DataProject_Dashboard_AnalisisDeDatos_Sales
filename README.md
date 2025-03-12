# Proyecto de Análisis de las ventas de coches en EE.UU
<div style="text-align: center;">
    <img src="Img/portada.png" alt="portada" />
</div>

Este proyecto tiene como objetivo analizar las tendencias de ventas de coches, utilizando datos históricos de los años 2022 a 2023 y mostrando los resultados en un dashboard interactivo.    

## Descripción del proyecto
El análisis de las ventas de coches en los estados unidos durante los años 2022 y 2023 busca identificar tendencias, patrones de compra y factores que influyen en el mercado automovilístico.  

Dentro del fichero car_sales.docx se encuentra el detalle sobre cada punto.

## Estructura del proyecto
```
DataProject_Dashboard_AnalisisDeDatos_Sales
├─ Data                         #Carpeta con los archivos utilizados
│  ├─ 1-Data_raw                    #Carpeta con los archivos originales
│  │  ├─ csv
│  │  │  └─ car sales.csv
│  │  └─ excel
│  │     └─ car_sales.xlsx
│  ├─ 2-Datos_transformados         #Carpeta con los datos transformados
│  │  └─ car_sales_transformados.xlsx
│  ├─ 3-Data_analisis               #Carpeta con los archivos utilizados
│  │  ├─ analisis_descriptivo_cat_temp_ventas.xlsx
│  │  ├─ analisis_descriptivo_numericas_ventas.xlsx
│  │  └─ car_sales_analisis_descriptivo.xlsx
│  ├─ 4-Datos_dashboard             #Carpeta con el dashboard final
│  │  └─ dashboard.xlsx
│  └─ Car_sales.docx
├─ Img                              #Carpeta con las imágenes utilizadas en el readme-md
│  ├─ dashboard.png
│  └─ portada.png
└─ README.md
```

## Datos
Descargamos el fichero desde la URL https://www.kaggle.com/datasets/safaeahb/car-sales-analysis-dashboard?select=car+sales.csv    

## Tecnologías Utilizadas
- Excel

## Estructura de datos

El archivo de datos original consta de las siguientes columnas:  
- **Car_id:** Identificador único de la venta.  
- **Date:** Fecha de la venta del vehículo.
- **Customer_Name:** Nombre del cliente que ha comprado el coche.
- **Gender:** Género del cliente que ha comprado el coche.
- **Annual Income:** Ingresos anuales del comprador del coche.
- **Dealer_Name:** Nombre del concesionario.
- **Company:** Marca del coche que se ha vendido.
- **Model:** Modelo del coche que se ha vendido.
- **Engine:** Tipo de motor del coche vendido. 
- **Transmission:** Tipo de transmisión del coche.
- **Color:** Color del coche.
- **Price ($):** Precio que ha costado el coche.
- **Dealer_No:** Número del concesionario.
- **Body Style:** Estilo de la carrocería del coche.
- **Phone:** Teléfono. Puede que sea el teléfono del comprador del coche. Es una columna irrevelente, así que no le vamos a dar importancia.
- **Dealer_Region:** Región del concesionario.


## Desarrollo del proyecto

* Entendimiento general del conjunto de datos y de las columnas.
* Eliminación de columnas, establecimiento del tipo de los datos y normalización de los datos.
   - Eliminamos las columnas customer_name, delaer_no y phone.  
   - Las columnas no tienen valores nulos y no tenemos filas duplicadas.
   - Todos los datos están normalizados.

    <br>
* Análisis descriptivo de las columnas numéricas.
    - Realizamos el análisis sobre las columnas:  
        - Annual Income.
        - Price ($).

    <br>
* Análisis descriptivo de las columnas categóricas y temporales.
    - Analizamos las siguientes columnas categóricas:
        - Gender.
        - Company.
        - Engine.
        - Transmission.
        - Color.
        - Body Stsyle
        - Dealer Region.

    - Analizamos la columna de tipo fecha:
        - Date.

    <br>
* Análisis descriptivo de las columnas numéricas y la columna objetivo.
    - Realizamos el análisis sobre las columnas:  
        - Annual Income.
        - Price ($).

    <br>
* Análisis descriptivo de las columnas categóricas y temporales. Creación de nuevas columnas.
    - Analizamos las siguientes columnas categóricas:
        - Gender.
        - Company.
        - Color.
        - Body Stsyle

    - Creamos una columna nueva:
        - Annual Income Type.

    - Analizamos las columnas de tipo fecha:
        - Sales / year.
        - Sales / Trim.
        - Sales / Month.

    <br>
* Elección de las columnas relevantes para el dashboard.

    <br>
* Creación del dashboard.
    - KPI:
        - Total ventas.    
        - Importe de las ventas.    
        - Importe medio de las ventas

    - Segmentadores:  
        - Gender.  
        - Transmision.  
        - Color.  
        - Year.  
        - Month. 

    - Gráficos:  
        - Company.  
        - Annual Income Type. 
        - Body style.   
    - Gráfico temporal:
        - Date
 
        

## Dashboard
<div style="text-align: center;">
    <img src="Img/dashboard.png" alt="dashboard" />
</div>

## Conclusiones
- Existe una tendencia al alza en la ventas, ya que 2023 supera en ventas al año 2022.  
- Los meses donde más coches se compran son los meses de final de año.  
- Las marcas americanas son las marcas con mayores ventas.  
- Los coches de tipo de SUV son los favoritos de los compradores.  
- El perfil de comprador de coches son los que tienen ingresos superiores.

## Contribuciones
Las contribuciones a este proyecto son bienvenidas. Si tienes alguna sugerencia, mejora o corrección, no dudes en ponerte en contacto o enviar tus ideas.

## Autor
Sergio Salmerón - [GitHub Profile](https://github.com/SergioSalm)