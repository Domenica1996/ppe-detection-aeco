# ppe-detection-aeco
# Detección de Equipos de Protección Personal (EPP) en imágenes de obra usando YOLOv8

## Problema AECO

El sector AECO (Architecture, Engineering, Construction and Operations) presenta una alta incidencia de accidentes laborales en obras. Muchos de estos accidentes se relacionan con la falta de uso de Equipos de Protección Personal (EPP) y con la escasa trazabilidad de condiciones de seguridad en obra.

Este proyecto explora el uso de visión computacional para detectar automáticamente elementos de seguridad en imágenes de obra.

## Criterios de éxito

El objetivo del proyecto es:

- entrenar un modelo reproducible en Google Colab,
- detectar correctamente personas y elementos de EPP,
- documentar métricas, evidencias visuales y limitaciones del modelo.

## Clases del modelo

Las clases utilizadas son:

- person
- helmet
- vest
- security_boots

## Reglas de etiquetado

- person: persona visible en la escena
- helmet: casco de seguridad visible
- vest: chaleco reflectante visible
- security_boots: botas de seguridad visibles

## Dataset

- Fuente: Roboflow
- Formato: YOLOv8
- Split: 80% entrenamiento / 20% validación
- Enlace al dataset: [PEGAR LINK DE ROBOFLOW]
- Versión del dataset: [COMPLETAR]

## Cómo reproducir en Google Colab

1. Abrir el notebook principal desde la carpeta `/notebooks/`.
2. Ejecutar las celdas de instalación de dependencias.
3. Descargar el dataset desde Roboflow.
4. Entrenar el modelo YOLOv8 o cargar pesos ya entrenados si corresponde.
5. Ejecutar validación.
6. Ejecutar inferencia en imágenes de validación e imágenes nuevas.
7. Revisar métricas, curvas y resultados guardados en `/results/`.

## Resumen de resultados

Métricas principales del modelo:

- Precision: [COMPLETAR]
- Recall: [COMPLETAR]
- mAP50: [COMPLETAR]
- mAP50-95: [COMPLETAR]

### Conclusiones clave

1. El modelo detecta correctamente personas y parte de los elementos de seguridad.
2. Los objetos pequeños, como cascos, presentan mayor dificultad de detección.
3. La mejora del balance de clases y de las anotaciones podría aumentar el recall.

## Checklist de Reproducibilidad

- Dataset / versión: 4
- Enlace al dataset: https://app.roboflow.com/domenicas-workspace/m4t3/4
- Variante del modelo: YOLOv8s
- epochs: 80
- batch: 16
- imgsz: 640
- versión de ultralytics: 8.2.103

## Estructura del repositorio

- `/notebooks/`: notebooks de entrenamiento, evaluación e inferencia
- `/docs/`: problema, clases, análisis de errores y gobernanza
- `/results/`: curvas, métricas y ejemplos de predicción
