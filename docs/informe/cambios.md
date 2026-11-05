# Cambios al informe preliminar

Archivos: `informePreliminar.odt` (original, sin tocar) → `informe_corregido.odt` y `informe_corregido.docx`.

## Qué se conservó sin cambios
- Estructura, numeración de secciones 1–17 y anexos A y B, y las 17 tablas (345 celdas, mismo número de filas y columnas).
- Todos los IDs (RF01–12, RNF01–10, HU01–06, N1–N9, O1–O6, D01–D12, P1–P5, P01–P14, S1–S8, E1–E4), las referencias [A1–A5, V1, V2, T1–T7, L1–L5] y las 15 marcas de tiempo de V1/V2. Se comprobó por script que no se perdió ni se agregó ninguna.
- Cifras, normas, fechas, celdas del HDU (K8, A19, etc.) y la sección 17 (Referencias), que no se tocó.
- La portada ("Por completar por el equipo") sigue igual.

## Cambios que afectan estructura (avisados)
1. **Sección 9 duplicada.** Se eliminó el encabezado «9 HISTORIAS DE USUARIO CONTINUACIÓN». HU04, HU05 y HU06 quedan bajo la sección 9, en orden, sin cambiar sus IDs ni su contenido.
2. **«HU02–04» → «HU02–HU04»** en el párrafo de épicas (solo claridad).
3. **Cinco porqués:** las preguntas de la tabla ahora llevan signos de interrogación («¿Por qué…?»).

## Cambios de redacción por sección
Criterio general: frases más cortas, voz activa, primera persona plural donde el equipo decide («proponemos», «usaremos»), menos «se propone / se establece / se determina», y sin cambiar el sentido ni los hechos.

| Sección | Qué se cambió y por qué |
|---|---|
| Portada | Sin cambios. |
| 1 Resumen ejecutivo | Se separó la necesidad de la propuesta, se pasó a voz activa y se explicó OCR en una frase. |
| 2 Introducción | Se redujo el lenguaje recargado; se dejó explícito que las entrevistas son material aportado, no realizado por el equipo. |
| 3 Contexto y causa raíz | Se explicó **SII** al primer uso. Se corrigieron las preguntas de los cinco porqués. Se acortaron respuestas conservando cada cita V2. |
| 4 Objetivos y alcance | Se reescribieron la lista de alcance, los límites y los «por confirmar». Se agregó que las actividades de levantamiento pendientes «no se han realizado». |
| 5 Necesidades | Se acortaron las justificaciones. Se explicó **SSDF** al primer uso. |
| 6 Tendencias | Se explicó **DevSecOps**, **Zero Trust** y **monolito modular** la primera vez que aparecen. |
| 7 Requerimientos funcionales | Concordancia y puntuación en las 12 filas; se separó «RF08 y RF09» en la trazabilidad. |
| 8 Requerimientos no funcionales | Se explicó **p95** y **TLS** al primer uso. Se aclararon redacciones de RNF02, RNF05 y RNF10. |
| 9 Historias de usuario | Se completó «Dado/Cuando/Entonces» con artículos y concordancia. Se explicó **HU**, **CRUD**, **épicas** y política **atómica (todo o nada)**. Se fusionó la sección duplicada. |
| 10 Reglas y decisiones | Se explicó **DJ (declaración jurada)**, **baja lógica**, **float** y **hash** al primer uso. Se conservaron intactas las referencias a celdas del HDU. |
| 11 Metodologías | Se acortaron la comparación y la elección justificada. La conclusión no cambió. |
| 12 Aplicación | Se reescribió la tabla de actividades y la de responsabilidades (P1–P5); sin cambios de contenido. |
| 13 Seguridad e impacto ético | Se reescribieron las 24 celdas de S1–S8 con voz más directa; se mantuvieron las referencias [T2], [T7]. |
| 14 Marco normativo | Se acortaron; no se tocó ninguna fecha ni norma. La afirmación sobre el Decreto 7 **no se verificó** (ver `pendientes_equipo.md`). |
| 15 Propuesta | Se explicaron **Django, PostgreSQL (SQL), MongoDB (NoSQL)** e **idempotencia**. Se dejó explícito el lenguaje y el tipo de base de datos. |
| 16 Validación | Se acortaron las 12 filas de pruebas; se explicó **rollback**. Los IDs P01–P14 no cambian. |
| 17 Referencias | Sin cambios. |
| Anexo A | Reescritura menor de las 15 filas y de los párrafos finales. Se verificó que la suma es 100 puntos (90 + 10). |
| Anexo B | Se reescribieron las 8 respuestas con voz más natural. |

## Qué NO se corrigió a propósito (solo se avisa)
Está en `pendientes_equipo.md`: IDs que no calzan, códigos de asignatura, discrepancias entre la guía y el enunciado, marcas de tiempo de V2 que no calzan con la transcripción y los vacíos respecto a la guía.

## Limitaciones
- No hay LibreOffice instalado: no pude abrir el `.odt` para revisar visualmente tablas y anchos de columna. La integridad se verificó sobre el XML (bien formado, mismo número de tablas y celdas).
- El `.docx` se generó con pandoc a partir del `.odt` corregido: conserva texto, tablas y encabezados, pero puede perder detalles de formato (estilos, anchos, colores). Conviene revisarlo en Word antes de entregar.
