# Análisis de errores del modelo

A continuación se presentan algunos ejemplos de errores detectados durante la evaluación visual del modelo.

## Falsos positivos

1. Detección de casco en objetos de forma similar  
   En algunas imágenes el modelo detecta cascos en objetos que tienen formas o colores similares.

2. Detección de chaleco en ropa de colores brillantes  
   Algunas prendas de colores intensos pueden ser clasificadas incorrectamente como chalecos de seguridad.

3. Detección de persona en objetos del fondo  
   En ciertos casos el modelo interpreta formas en el fondo como si fueran personas.

## Falsos negativos

1. Casco no detectado cuando está parcialmente oculto  
   Cuando el casco está cubierto parcialmente por otros objetos, el modelo puede no detectarlo.

2. Botas de seguridad no detectadas cuando aparecen pequeñas en la imagen  
   Cuando las personas aparecen muy lejos en la escena, el tamaño de las botas puede ser demasiado pequeño para ser detectado.

3. Chaleco no detectado en condiciones de baja iluminación  
   En zonas con sombras o poca luz el modelo puede no identificar correctamente el chaleco.

## Mejoras prioritarias del dataset

1. Aumentar la diversidad del dataset  
   Incluir imágenes de distintas obras, ángulos de cámara y condiciones de iluminación.

2. Mejorar el equilibrio entre clases  
   Incorporar más ejemplos de clases menos representadas, como botas de seguridad.

3. Incluir más ejemplos con oclusiones  
   Agregar imágenes donde los elementos de seguridad estén parcialmente cubiertos.
