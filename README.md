# Generador de Unidades Didácticas - Matemática Secundaria

Este proyecto sirve para trabajar con Codex y automatizar la generación de unidades didácticas en Word, siguiendo el patrón institucional del usuario.

## 1. Qué contiene este paquete

- `AGENTS.md`: instrucciones permanentes para Codex.
- `datos/unidad_2.json`: información pedagógica estructurada de la Unidad 2.
- `scripts/generar_unidad.py`: script que genera el documento Word.
- `recursos/`: logotipos y firma del docente.
- `plantillas/`: unidad modelo oficial.
- `referencias/`: planificación anual y situación significativa.
- `docs/estandares_matematica_ciclo_vi.md`: estándares de C2 y C4 para segundo de secundaria.
- `salida/`: carpeta donde se guarda el documento generado.

## 2. Cómo generar la Unidad 2

Desde la carpeta principal del proyecto, ejecutar:

```bash
pip install -r requirements.txt
python scripts/generar_unidad.py datos/unidad_2.json
```

El archivo se generará en:

```text
salida/UNIDAD_DE_APRENDIZAJE_N2_SEGUNDO_2026.docx
```

## 3. Cómo usarlo con Codex

1. Subir este proyecto a un repositorio de GitHub.
2. Abrir el repositorio desde Codex.
3. Pedir a Codex que lea `AGENTS.md` antes de realizar cambios.
4. Darle una tarea específica, por ejemplo:

```text
Lee AGENTS.md, revisa la plantilla de la Unidad 1 y mejora el script scripts/generar_unidad.py para que el Word generado se parezca más al formato visual de plantillas/UNIDAD_DE_APRENDIZAJE_N1_SEGUNDO.docx. Luego ejecuta python scripts/generar_unidad.py datos/unidad_2.json y valida que el archivo se cree correctamente.
```

## 4. Prompt para generar una nueva unidad

Cuando quieras crear otra unidad, puedes pedir:

```text
Crea el archivo datos/unidad_3.json usando la planificación anual y el patrón de datos/unidad_2.json. Luego genera el Word con el formato oficial. Mantén coherencia entre situación significativa, competencias, criterios, evidencias, secuencia de sesiones, producto e instrumentos.
```

## 5. Recomendación de trabajo

- ChatGPT puede ayudarte a redactar y validar pedagógicamente cada unidad.
- Codex puede automatizar el formato, mejorar el script y generar archivos Word repetibles.

