#Proyecto de Reconocimiento de Entidades Nombradas (NER)

Este proyecto está diseñado para procesar y entrenar modelos de Reconocimiento de Entidades Nombradas (NER) utilizando anotaciones en formato JSON. A continuación, se describe la estructura del proyecto y el propósito de cada archivo y carpeta.

---

## **Estructura del Proyecto**

### **1_procesamiento_anotaciones/**
Carpeta destinada al procesamiento de anotaciones en formato JSON. Contiene los siguientes archivos y carpetas:

- **`procesamiento_anotaciones.ipynb`**: Cuaderno de Jupyter que analiza los archivos JSON en busca de errores, como espacios en blanco inválidos en las entidades. También genera un archivo de log con los resultados.
- **`input_annotations/`**: DEBES crear esta carpeta que contiene los archivos JSON con las anotaciones originales.
- **`logs/`**: Carpeta donde se almacenan los registros generados durante el procesamiento.

---

### **2_entrenamiento_NER/**
Carpeta destinada al entrenamiento del modelo NER. Contiene los siguientes archivos:

- **`entrenamiento_NER.ipynb`**: Cuaderno de Jupyter que convierte las anotaciones procesadas en un formato compatible con spaCy, divide los datos en conjuntos de entrenamiento y validación, y entrena el modelo.
- **`config.cfg`**: Archivo de configuración para el entrenamiento del modelo spaCy. Define los parámetros del modelo, las rutas de los datos y las configuraciones de entrenamiento.

---

## **Cómo usar este proyecto**

### **1. Procesar anotaciones**
1. Coloca los archivos JSON con anotaciones en la carpeta `1_procesamiento_anotaciones/input_annotations/`.
2. Abre el archivo `procesamiento_anotaciones.ipynb` en Jupyter Notebook.
3. Ejecuta las celdas para analizar las anotaciones y generar un archivo de log con los resultados.

### **2. Entrenar el modelo**
1. Asegúrate de que las anotaciones procesadas estén en el formato compatible con spaCy.
2. Abre el archivo `entrenamiento_NER.ipynb` en Jupyter Notebook.
3. Ejecuta las celdas para dividir los datos, entrenar el modelo y guardar los resultados.

---

## **Requisitos**

- Python 3.8 o superior
- Bibliotecas necesarias:
  - `spacy`
  - `scikit-learn`
  - `ipywidgets`
  - `torch` (si se utiliza un modelo basado en transformadores)
- Jupyter Notebook para ejecutar los cuadernos.

---

## **Notas adicionales**

- El archivo `config.cfg` debe ser configurado correctamente antes de entrenar el modelo.

