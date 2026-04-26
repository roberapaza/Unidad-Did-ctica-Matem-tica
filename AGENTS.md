# Instrucciones para Codex: Generador de Unidades Didácticas

Este repositorio genera unidades didácticas de Matemática para secundaria en formato Word (.docx), siguiendo el patrón institucional del usuario.

## Objetivo principal
Automatizar la redacción y el formato de unidades de aprendizaje a partir de datos estructurados en JSON, respetando la planificación anual, el currículo nacional y la plantilla oficial.

## Reglas de formato obligatorio
- Documento en orientación horizontal A4.
- Márgenes: superior 2.83 cm, inferior 1.27 cm, izquierdo 1.27 cm, derecho 1.27 cm.
- Fuente general: Calibri 11.
- Título principal: Calibri 20, centrado, negrita y subrayado.
- Título contextual de la unidad: Calibri 20, centrado, negrita, color azul #0000FF.
- Encabezados de tablas con color de fondo #D9E2F3 o #8EAADB cuando corresponda.
- Tablas con bordes visibles, ajustadas al ancho de página.
- Incluir logo institucional en encabezado izquierdo o central.
- Incluir logo de Khan Academy en encabezado derecho.
- Incluir firma del docente ROBERTO APAZA ROBLES al final cuando el recurso exista.
- Mantener la frase sobre Khan Academy en negrita y color rojo cuando aparezca en criterios transversales.

## Estructura obligatoria de cada unidad
1. Título: UNIDAD DE APRENDIZAJE N° ...
2. Título contextual de la unidad entre comillas.
3. Datos informativos.
4. I. Situación significativa.
5. Tabla de problemática de contexto, necesidades/intereses, competencias seleccionadas y producto de la unidad.
6. II. Enfoques transversales.
7. III. Competencias transversales.
8. IV. Matriz de planificación: estándar / competencia / capacidades / criterios / evidencias / instrumentos.
9. V. Secuencia de sesiones.
10. VI. Producto integrado de la unidad.
11. VII. Instrumentos de evaluación.
12. VIII. Materiales y recursos.
13. Firmas de docentes responsables.

## Reglas pedagógicas
- La situación significativa debe partir del contexto real de la comunidad educativa MVRHT N.° 0148.
- Debe vincular problema priorizado, necesidad/interés, competencias, contenidos matemáticos, producto y preguntas retadoras.
- Los criterios deben derivarse de las capacidades de la competencia.
- Las evidencias deben ser observables y relacionadas con el producto de unidad.
- Los propósitos de sesión deben iniciar con: "Que los estudiantes...".
- No inventar estándares si existen en los documentos de referencia. Revisar primero `docs/estandares_matematica_ciclo_vi.md` y las referencias.
- Mantener coherencia entre situación significativa, competencias, criterios, secuencia de sesiones, evidencias e instrumentos.

## Comandos esperados
Para generar la Unidad 2:

```bash
python scripts/generar_unidad.py datos/unidad_2.json
```

El archivo final debe guardarse en la carpeta `salida/`.

## Mantenimiento
- Si se agregan nuevas unidades, crear un archivo JSON por unidad en `datos/`.
- Si cambia el patrón visual, actualizar primero este archivo y luego el script `scripts/generar_unidad.py`.
