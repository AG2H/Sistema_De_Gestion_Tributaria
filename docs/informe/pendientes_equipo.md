# Pendientes del equipo y avisos

Todo lo de esta lista **no se tocó ni se rellenó** en `informe_corregido.odt`: solo el equipo o el docente pueden resolverlo.

## A. Datos que solo el equipo puede completar
- [ ] **Integrantes y sección** (portada).
- [ ] **Contraparte del grupo** (portada).
- [ ] **Fecha del informe.** Dice 1 de noviembre de 2026. Hoy es 4 de noviembre y la entrega E1 es el 7 de noviembre.
- [ ] **Responsables P1–P5:** nombres y capacidad horaria. Con cuatro integrantes, P2 y P4 comparten P5.
- [ ] **Aviso de grupo:** el informe dice que vence el 1 de noviembre (según A1). Confirmar que se hizo.
- [ ] **Defensa individual:** cada integrante debe preparar las 8 preguntas del Anexo B.

## B. Qué falta o está débil frente a la guía (sin rellenar)
**Actividad 1 – Antecedentes y normativa**
- Antecedentes tecnológicos y administrativos (infraestructura, recursos, restricciones, cultura institucional): solo hay una lista «por confirmar» en la sección 4. **Débil.**
- Normativa: cubierta (Ley 19.628/21.719, 21.663, SII, NIST, OWASP).

**Actividad 2 – Levantamiento de datos y requerimientos**
- Planificación del levantamiento: un solo párrafo; solo menciona entrevista, revisión de CSV y observación. **No hay encuestas ni técnicas de análisis, ni recursos y tiempos.** La guía pide además **asignar tareas específicas por integrante**: no aparece. **Débil.**
- RF/RNF: cubiertos (12 y 10).
- Cinco porqués: cubiertos.

**Actividad 3 – Épicas, historias y priorización**
- **Épicas:** solo se nombran en un párrafo; falta una tabla con nombre y descripción. **Débil.**
- **Product backlog priorizado:** descrito en texto (sección 12), no como lista ordenada.
- **MoSCoW poco discriminante:** N1–N9 son todas «M» y las seis HU también. Conviene justificar qué quedaría fuera de un mínimo.
- La guía pide un enfoque de **producto mínimo viable (PMV)**; el informe no lo nombra.
- Historias de usuario: 6, con Dado/Cuando/Entonces. Cubierto.

**Actividad 4 – Metodologías y seguridad**
- **Lenguaje:** Python/Django (propuesta). Cubierto.
- **Tipo de base de datos:** PostgreSQL (SQL) + MongoDB (NoSQL). Cubierto.
- **Tipo de almacenamiento (local, hosting o nube): no está decidido.** Dice «almacenamiento privado» y «nube… proveedor por definir». **Falta.**
- **Arquitectura e infraestructura** (punto d de la guía): monolito modular y vistas 4+1 en E2; **no hay infraestructura definida** (servidor, entornos, despliegue). **Débil.**
- Metodologías y seguridad con impacto ético (S1–S8): cubiertas.
- La guía menciona Design Thinking, DevOps y Agile como metodologías emergentes; el informe trata Kanban/iterativo y DevSecOps, no Design Thinking.

**Formato de entrega**
- La guía pide: Resumen ejecutivo, Introducción, Desarrollo (4 apartados con los nombres de las actividades) y Conclusiones y recomendaciones. El informe tiene 17 secciones sin etiquetar cuáles son las cuatro actividades. Considerar una tabla que las asocie (el Anexo A solo asocia con la rúbrica).

**Criterios 1.1.1–1.1.5:** los cinco tienen evidencia (ver Anexo A). Lo más flojo: 1.1.1 (buenas prácticas de la industria apoyadas solo en SSDF/OWASP) y 1.1.2 (todas las HU en «M»).

## C. Códigos y discrepancias a confirmar con el docente (no se cambiaron)
- **Código de asignatura:** la guía y el informe dicen **TIHV43**; el texto de evaluación de la guía dice **TIHI43** («Proyecto Integrado TIHI43»).
- **Tamaño de grupo:** guía = 2 o 3 estudiantes; enunciado/clase (según el informe) = 4 o 5.
- **Hora límite:** guía = 23:00 h; el informe cita el enunciado con 23:59.
- **Formato de entrega:** guía = archivo `.rar` llamado `Apellido1_Apellido2_Seccion` subido a AAI, sin correo; el informe cita «Word/PDF» según el enunciado.
- **Fecha de la guía:** «Primavera 2025».

## D. Incoherencias internas (se avisan, no se corrigieron)
1. **RF10 cita HU05**, pero HU05 no lista RF10 entre sus RF.
2. **RF12 cita HU05/06**, pero HU06 no lista RF12 (HU05 sí).
3. **N5** no lista RF12, aunque RF12 cita N5.
4. **Nombres que se confunden:** las responsabilidades se llaman P1–P5 y las pruebas P01–P14 (por ejemplo, «P1/P2» en riesgos y «P08/P14» en N9). Sugerencia: renombrar las responsabilidades (por ejemplo R1–R5). No lo hice porque cambia IDs.
5. **Pruebas sin cobertura explícita:** RF03, RF10, RF12 y RNF08 no tienen una prueba asociada en la sección 16.
6. **P13/P14** («descarga ajena denegada») están asociadas a RF11/RNF05, pero lo que prueban es aislamiento (RNF01).
7. **Tablas:** todas las filas de las 17 tablas tienen el mismo número de celdas; no encontré filas desalineadas. No pude revisar anchos de columna visualmente (no hay LibreOffice).
8. **«HDU»:** se usa sin definir. No inventé su significado; confirmar y expandirlo en el primer uso.
9. **«Actualización anual»** en sección 11: el video dice «actualización constante» (ver `analisis_entrevista_vs_informe.md`).

## E. Datos por confirmar con el cliente o la contraparte
- Decisiones **D01–D12** (cálculos, catálogos, formatos, clave de actualización, baja local, documento histórico).
- **¿Se debe cargar directamente desde una declaración jurada?** El video lo menciona; el informe solo cubre monto y factor.
- Volúmenes, sistemas existentes, infraestructura, presupuesto, política de acceso y año tributario.
- Plazo de retención del archivo histórico, y si se conserva el original o una reconstrucción.
- Metas propuestas: p95 ≤2 s con 10.000 registros (RNF04), restauración ≤60 min y pérdida tolerable de 24 h (RNF05), margen del 20 %.
- Proveedor y tipo de almacenamiento; infraestructura de despliegue.

## F. Fuentes que no pude verificar
- **Decreto 7 (referencia L5):** el informe afirma que el enlace de la guía corresponde a un reglamento de protección de la niñez, no a la norma de ciberseguridad. Intenté abrir la página de la BCN pero no cargó (requiere JavaScript). **No lo verifiqué.** Revisar antes de entregar: es una afirmación sobre una norma.
- **L1–L4** (Ley 19.628/21.719, Ley 21.663, Res. Ex. SII 85/2024): no las verifiqué en línea. El informe fecha la vigencia de la Ley 21.719 al 1 de diciembre de 2026.
- **V1:** no tengo el video; no pude comprobar sus citas (00:10–00:52, 02:19–02:39, 03:31–04:12) ni la duración 04:25.
- **Transcripción de V2:** las citas con minutos exactos deben revisarse escuchando el video en las palabras marcadas `[?]`.
