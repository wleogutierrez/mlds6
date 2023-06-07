<style>
    .rendered_html h1, .rendered_html h2, .rendered_html h3, .rendered_html h4, .rendered_html h5, .rendered_html h6 {
        counter-reset: none !important;
    }
</style>

# Project Charter - Entendimiento del Negocio
_______

## Nombre del Proyecto
____
Ventas en tiendas - Pronóstico de series temporales
<br>

## Objetivo del Proyecto 
____

El objetivo de este proyecto es pronosticar las ventas de las tiendas a partir de los datos de Corporación Favorita, un gran minorista de comestibles con sede en Ecuador.
<br>

## Alcance del Proyecto
___
### Incluye:

* **Descripción de los datos disponibles:**
<br>

Para el desarrollo de este proyecto se utilizará el conjunto de datos [Store Sales - Time Series Forecasting](https://www.kaggle.com/competitions/store-sales-time-series-forecasting/overview) disponible en kaggle.<br>
#### **train.csv**
Los datos de entrenamiento, que incluyen series temporales de las características **store_nbr**, **family** y **onpromotion**, así como las ventas objetivo.
* **store_nbr:** identifica la tienda en la que se venden los productos.
* **family:** identifica el tipo de producto vendido.
* **sales:** total de ventas de una familia de productos en una tienda concreta en una fecha determinada. Los valores fraccionarios son posibles ya que los productos pueden venderse en unidades fraccionarias (1,5 kg de queso, por ejemplo, frente a 1 bolsa de patatas fritas).
* **onpromotion:** da el número total de artículos de una familia de productos que estaban en promoción en una tienda en una fecha determinada.
<br>

#### **test.csv**
* Los datos de prueba contienen las mismas características que los datos de entrenamiento. Predecirá las ventas objetivo para las fechas de este archivo.
* Las fechas de los datos de prueba corresponden a los 15 días posteriores a la última fecha de los datos de entrenamiento.
<br>

#### **sample_submission.csv**
* Un archivo de envío de muestra en el formato correcto.
<br>

#### **stores.csv**

* Metadatos de la tienda, incluidos ciudad, estado, tipo y grupo.
* **cluster** es una agrupación de tiendas similares.<br>

#### **oil.csv**

Precio diario del petróleo. Incluye valores durante los periodos de datos de prueba y de entrenamiento. (Ecuador es un país dependiente del petróleo y su salud económica es muy vulnerable a las perturbaciones de los precios del petróleo).<br>

#### **holidays_events.csv**

Días festivos y eventos, con metadatos<br>

### **Descripción de los resultados esperados**<br>

Se espera el despliegue de un modelo que permita predecir las ventas de las tiendas <br>

### **Criterios de éxito del proyecto**<br>

Para que el proyecto sea culminado con éxito se requiere:

* una previsión más precisa la cual puede reducir el desperdicio de alimentos relacionado con el exceso de existencias y mejorar la satisfacción del cliente. 

### **Excluye:** 

Para el desarrollo del proyecto se replicará la línea base presentada por [TOM KELDENICH](https://www.kaggle.com/code/kelde9/darts-ensemble-stores-sales-forecasting)


### **Cronograma:**
______ 
<br>

|Etapa |Duracion |Fecha |
|--|--|--|
|Entendimiento del negocio y carga de datos	|1 semana| del 30 de Mayo al 6 de junio|
|Preprocesamiento,extracción de características y modelado|1 semana| del 30 de Mayo al 6 de junio|
|Despliegue del modelo | 1 Semana | del 30 de Mayo al 6 de junio|
|Evaluacion y monitoreo del modelo |1 Semana | del 30 de Mayo al 6 de junio|

<br>

### **Equipo del Proyecto**
___
* Leonardo Gutiérrez
