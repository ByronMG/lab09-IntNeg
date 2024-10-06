﻿# lab09-IntNeg
Instrucciones para ejecutar los análisis con Python
Requisitos previos
Python 3.6 o superior debe estar instalado en tu sistema.
Instalar las bibliotecas necesarias ejecutando el siguiente comando:
bash
Copiar código
pip install pandas scikit-learn matplotlib seaborn openpyxl
Nota: openpyxl es necesario para leer archivos de Excel en formato .xlsx.

Análisis 1: Clustering con K-Means y visualización de histogramas
Paso 1: Cargar y explorar los datos
El archivo de datos BI_Postulantes09-1.xlsx debe estar disponible en el mismo directorio que el script.
El código carga el archivo de Excel, inspecciona las hojas, y carga los datos de 'Hoja1' en un DataFrame para análisis.
Paso 2: Preparar los datos para K-Means
Se seleccionan columnas relevantes para el clustering: Apertura Nuevos Conoc., Nivel Organización, Participación Grupo Social, etc.
El algoritmo K-Means se aplica con 3 clústeres predeterminados, y los resultados se asignan a una nueva columna Cluster.
Paso 3: Graficar histogramas
Se generan histogramas de las variables Apertura Nuevos Conoc. y Grado Empatía, desglosados por los clústeres resultantes.
Los histogramas muestran la distribución de estas variables y los grupos asignados por el algoritmo.
Cómo ejecutar:
Asegúrate de tener el archivo BI_Postulantes09-1.xlsx en el directorio del script.
Ejecuta el código para ver los histogramas del análisis de K-Means:
bash
Copiar código
python clustering_kmeans.py
