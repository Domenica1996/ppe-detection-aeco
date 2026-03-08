# Checklist de gobernanza

## 1. Privacidad y consentimiento

Este proyecto utiliza imágenes para entrenar y evaluar un modelo de detección de Equipos de Protección Personal (EPP) en contextos de obra del sector AECO.

Consideraciones:
- Se debe verificar que las imágenes utilizadas puedan emplearse con fines académicos y de experimentación.
- Si las imágenes contienen personas identificables, su uso debe respetar las condiciones de privacidad y los derechos correspondientes.
- Este repositorio no busca recopilar información personal ni realizar identificación de individuos, sino detectar objetos y elementos de seguridad visibles en la imagen.

## 2. Minimización de datos

El proyecto utiliza únicamente las imágenes necesarias para entrenar, validar y probar el modelo de detección.

Medidas de minimización:
- No se recopilan datos personales adicionales.
- No se almacenan datos sensibles fuera de las imágenes originales utilizadas en el experimento.
- El repositorio incluye resultados, métricas y evidencias visuales necesarias para la evaluación del proyecto, evitando incluir contenido irrelevante.

## 3. Declaración de limitaciones

Este modelo no debe utilizarse como sistema autónomo de control de seguridad en obra.

No se recomienda su uso en los siguientes casos:
- Como única herramienta para fiscalización de cumplimiento de normas de seguridad.
- En entornos reales sin supervisión humana.
- En situaciones críticas donde un error de detección pueda generar riesgos importantes.
- En imágenes con condiciones muy distintas a las del dataset de entrenamiento, como baja iluminación extrema, oclusiones severas o puntos de vista muy diferentes.

El modelo debe entenderse como una herramienta experimental y académica de apoyo visual, no como un sistema definitivo de toma de decisiones.

## 4. Nota de riesgos: falsos negativos vs falsos positivos

### Falsos negativos (FN)
Un falso negativo ocurre cuando el modelo no detecta un elemento de seguridad que sí está presente, o no detecta correctamente una situación relevante.

Riesgo:
- Puede omitir casos importantes y dar una falsa sensación de cumplimiento o de ausencia de riesgo.
- En aplicaciones reales, este tipo de error puede ser especialmente problemático si se usa el modelo para supervisión de seguridad.

### Falsos positivos (FP)
Un falso positivo ocurre cuando el modelo detecta incorrectamente un objeto o elemento de seguridad que no corresponde.

Riesgo:
- Puede generar interpretaciones erróneas sobre la presencia de EPP.
- Puede disminuir la confianza en el sistema si ocurre con demasiada frecuencia.

### Consideración general
En un contexto de seguridad, los falsos negativos suelen ser más críticos que los falsos positivos, ya que implican omitir situaciones que podrían requerir atención.

## 5. Derechos del dataset

El dataset utilizado en este proyecto fue gestionado mediante Roboflow y corresponde a la versión documentada en el README del repositorio.

Se debe aclarar expresamente cuál es la situación del dataset:
- [ ] Dataset propio
- [ ] Dataset público
- [ ] Dataset licenciado para uso académico
- [ ] Otro (especificar)

Nota:
El uso del dataset debe respetar sus condiciones de origen, licencia y permisos de reutilización.

## 6. Licencia del proyecto

El código de este repositorio se distribuye bajo licencia MIT.

Esto aplica al código, documentación y estructura del proyecto, pero no reemplaza ni modifica los posibles derechos o restricciones asociados al dataset y a las imágenes utilizadas.
