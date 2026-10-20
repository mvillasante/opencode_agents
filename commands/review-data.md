---
description: Review commited data
---

Tu misión es revisar el diff de commit proporcionado contra la checklist especificada y generar un informe de revisión. Para lograrlo, debes:

- Leer y comprender completamente el archivo checklist.md, identificando cada criterio de verificación.
- Analizar el diff proporcionado, examinando cada archivo modificado, las líneas añadidas y eliminadas.
- Evaluar cada cambio del diff contra cada criterio de la checklist, determinando cumplimiento o incumplimiento.
- Documentar los hallazgos de forma estructurada, indicando el archivo, la línea o sección afectada y el criterio de la checklist involucrado.
- Clasificar cada hallazgo por severidad: crítico (bloqueante), mayor (requiere corrección) o menor (sugerencia de mejora).
- Proporcionar recomendaciones concretas y accionables para cada incumplimiento detectado.
- Señalar los aspectos positivos del diff que cumplen correctamente con la checklist.
- Generar un resumen ejecutivo con el veredicto general: aprobado, aprobado con observaciones o rechazado.
- Escribir el informe completo en el archivo review.md con formato Markdown estructurado.
- Si el diff o la checklist no son proporcionados, solicitar al usuario que los comparta antes de proceder.

## Context:
Este prompt se aplica a la revisión de commits en proyectos de software donde existe una checklist de calidad definida en checklist.md. El usuario proporcionará el diff del commit a revisar. El diff puede incluir múltiples archivos y tipos de cambios (adiciones, modificaciones, eliminaciones). Debes asumir que el diff es la fuente de verdad sobre los cambios realizados. El informe generado en review.md será utilizado por el autor del commit o por el equipo de revisión para decidir si el commit se aprueba o requiere correcciones. La audiencia del informe son desarrolladores con conocimiento técnico del proyecto.

## Format:

Archivo de Salida: El informe completo debe escribirse en review.md dentro de un bloque de código Markdown.

Estructura del Informe:

1. Resumen Ejecutivo: Veredicto general y conteo de hallazgos por severidad.
2. Hallazgos: Lista de incumplimientos, cada uno con: severidad, archivo/línea, criterio de checklist, descripción del problema, recomendación.
3. Aspectos Positivos: Lista de cumplimientos destacables.
4. Conclusión: Recomendación final y próximos pasos.

Severidad: Usa etiquetas [CRÍTICO], [MAYOR], [MENOR] para clasificar cada hallazgo.

Estilo: Técnico, directo, sin emojis ni texto conversacional fuera del bloque de código.

Longitud: Proporcional al tamaño del diff y número de hallazgos; sé exhaustivo pero conciso.
