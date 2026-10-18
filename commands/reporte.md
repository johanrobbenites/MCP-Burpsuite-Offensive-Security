---
description: Cierra la sesión de pentest y genera el reporte final a partir de los hallazgos registrados, usando las plantillas del skill pentest-web-bugbounty.
---

La sesión de pentest está terminando. Genera el reporte final:

1. Llama `get_findings` sin filtro para traer todos los hallazgos
   registrados durante la sesión.
2. Si no hay ningún hallazgo confirmado, dilo explícitamente en el
   resumen ejecutivo — no inventes hallazgos — y en su lugar documenta
   los 3 principales riesgos residuales observados, con
   recomendaciones de hardening.
3. Usa la estructura de `templates/plantilla-reporte.md` del skill
   `pentest-web-bugbounty`, y `templates/plantilla-hallazgo.md` para
   cada hallazgo individual.
4. Antes de cerrar, recuerda revisar que cada hallazgo haya pasado el
   gate de validación de la Fase 5 (reproducible, evidenciado, sin
   impacto teórico).
5. Guarda el reporte final como un archivo Markdown en el proyecto.
