# PhawAI_2025
# Clasificación de cáncer de pulmón en CT scans: estudio comparativo de tres modelos de transfer learning

Este repositorio contiene la implementación y evaluación de tres modelos de **transfer learning** (VGG16, ResNet50 y MobileNetV2) aplicados a la clasificación de imágenes de tomografía computarizada (CT) de tórax para la detección de cáncer de pulmón.

## Dataset
Se utilizó el dataset público **IQ-OTH/NCCD - Lung Cancer Dataset** disponible en Kaggle:  
[https://www.kaggle.com/datasets/adityamahimkar/iqothnccd-lung-cancer-dataset/data](https://www.kaggle.com/datasets/adityamahimkar/iqothnccd-lung-cancer-dataset/data)  

- Contiene 1190 imágenes correspondientes a 110 casos, clasificados en: **normal (55), benigno (15), maligno (40)**.  
- Las imágenes fueron recolectadas en hospitales especializados de Iraq, con consentimiento ético y anonimizadas antes del análisis.  

## Código Base
El código fue adaptado del notebook de **Garvit Gulati**:  
[VGG16_ResNet50_MobileNetV2](https://www.kaggle.com/code/garvitgulati/vgg16-resnet50-mobilenetv2/notebook) (Kaggle, 2024).  

Se realizaron ajustes en el preprocesamiento, entrenamiento y evaluación para adecuarlo a este dataset y objetivo de investigación.

## Cómo ejecutar en Colab
1. Abrir el notebook en Google Colab.  
2. En el menú superior: **Entorno de ejecución → Cambiar tipo de entorno de ejecución → Acelerador de hardware → GPU**.  
3. Ejecutar todas las celdas secuencialmente.  
4. Los gráficos de métricas, matrices de confusión y ejemplos de inferencia se mostrarán como salidas del notebook.  
5. No es necesario subir el dataset completo al repositorio; basta con descargarlo desde Kaggle y colocar la ruta correcta en las celdas de carga de datos.  

## Notas
- Todo el trabajo se realizó con fines **académicos y de investigación**.  
- Los resultados incluyen métricas de precisión, recall, F1-score y matriz de confusión para cada modelo.
