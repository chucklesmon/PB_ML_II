# Product Price Prediction on Amazon

This project applies Machine Learning to predict the price of products on Amazon based on their characteristics.

## Objective

Develop a model capable of estimating the price of new products using attributes such as category, brand, variants, and other properties.

## Dataset

The dataset contains data extracted via web scraping from Amazon products.

Data cleaning and variable transformation were performed to prepare a clean version of the dataset ready for modeling.

## Preprocessing

- Removal of irrelevant columns  
- Detection and treatment of outliers  
- Feature Engineering:  
  - Scaling  
  - Encoding of categorical variables  
  - Target transformation using Box-Cox  
  - New derived variables  
- Early Train/Test split to avoid data leakage

## Modeling

Several models were tested, and Linear Regression was identified as the best-performing model.

Testing of different models can be reviewed in `src/notebooks/pruebas.ipynb`.

## Future Improvements

- Add data from parameters not included in the initial dataset  
- Advanced text processing to better handle textual columns


## Project Structure

```plaintext
├── src/                # Project resources
    ├── data_sample/    # Dataset
    ├── img/            # Project images
    ├── models/         # Trained model(s)
    ├── notebooks/      # Notebooks with experiments
├── main.ipynb          # Main notebook summarizing and executing the project
├── presentacion.pdf    # Project presentation
├── README.md
```

--------------------------------------------------------------------------------------------------------------------------------------------------------------

# Predicción de Precios de Productos en Amazon

Este proyecto aplica Machine Learning predecir el precio de productos para Amazon a partir de sus características. 


## Objetivo

Desarrollar un modelo capaz de estimar el precio de productos nuevos basándose en atributos como categoría, marca, variantes, y otras propiedades.


## Dataset

El dataset contiene datos extraídos mediante scraping de productos de Amazon.

Se realiza limpieza de datos y transformación de variables para dejar una versión tratada del dataset lista para modelar.


## Preprocesado

- Eliminación de columnas irrelevantes.
- Detección y tratamiento de outliers.
- Feature Engineering:
  - Escalado
  - Encoding de variables categóricas
  - Transformación del target con Box-Cox
  - Nuevas variables derivadas
- División de datos en Train/Test desde el inicio para no tener en cuenta datos de test en train.


## Modelado

Se probaron varios modelos y se identificó Regresión Lineal como el mejor.

La prueba de los distintos modelos se puede revisar en (src/notebooks/pruebas.ipynb)


## Modificaciones a Futuro

- Añadir datos de parámetros no contemplados en el dataset inicial.
- Procesamiento de texto avanzado para tratar mejor las columnas.



## Estructura del proyecto

```plaintext
├── src/                # Contiene recursos del proyecto
    ├── data_sample/    # Contiene el dataset
    ├── img/            # Imágenes del proyecto
    ├── models/         # Modelo
    ├── notebooks/      # Notebooks con pruebas
├── main.ipynb          # Notebook principal, donde se resume y ejecuta todo el proyecto
├── presentacion.pdf    # Presentación del proyecto
├── README.md
```
