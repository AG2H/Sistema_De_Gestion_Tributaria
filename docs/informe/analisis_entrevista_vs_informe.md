# Análisis de la entrevista (V2) frente al informe y a la guía

Fuente: `entrevista_leiva_tiempos.txt` (transcripción propia con faster-whisper, modelo **small**, español; 45 segmentos, duración 03:44).

## Cómo leer los tiempos
- Hay voz entre **00:08–01:49** (presentación del caso) y **01:56–03:36** (respuestas sobre fuentes y almacenamiento). Entre 00:00–00:08 y 01:49–01:56 no hay voz.
- Los tiempos de cada segmento son aproximados (±1–2 s) porque dependen de cómo Whisper corta las frases.
- 29 palabras están marcadas `[?]`. Antes de citar en el informe académico, conviene escuchar esos puntos. Ejemplos: «Noam» (Nuam), «Leyva» (Leiva), «desclaves» (¿claves?), «búsqueda deficientes» (¿eficiente?), «una de jota» (¿DJ?), «recertificados», «opundar».
- El video es la entrevista V2. **V1 no lo tengo**, así que no pude verificar nada de V1.

## 1. Lo que el video dice y el informe recoge (concuerda)
| Lo dicho en el video | Dónde está en el informe |
|---|---|
| Mantenedor de calificaciones tributarias «robusto y de fácil uso» (00:45–00:55) | Objetivo general; O5; N7; RNF07 |
| Cargar, modificar y gestionar calificaciones basadas en montos convertidos en factores (00:50–01:00) | O1, O2; RF03–RF07; HU02, HU03 |
| Funcionalidades: búsqueda eficiente, crear/modificar/eliminar, carga masiva con archivos (01:04–01:14) | RF02, RF03, RF05, RF06, RF07; RNF04 |
| Confiabilidad y actualización constante (01:14–01:20) | RNF02, RNF03; O2 |
| Integrar fuentes de forma segura y eficiente; analizar requerimientos y riesgos (01:20–01:33) | Secciones 7–8, 13, 16 |
| Expectativas: optimizar gestión, facilitar el trabajo, integridad y trazabilidad, reducir tiempos y errores (01:36–01:45) | Sección 11 («peticiones del cliente»); O5; RF08; sección 16 (medición) |
| Fuentes públicas de emisores; DJ y certificados; el SII recibe la DJ (01:56–02:31) | Sección 3 (actores); sección 14; Anexo B-6 |
| Certificados en PDF sin formato fijo y orden distinto a la DJ; hoy no es automatizable (02:54–03:14) | Cinco porqués 1–3; OCR como «C» y fuera del alcance mínimo |
| Almacenamiento anual; se pueden pedir DJ de años anteriores (03:14–03:36) | N5, O4, RF11, RNF09, HU06, D12 |

## 2. Lo que el video dice y el informe no refleja bien
1. **«Por monto, por factor o directamente de una declaración jurada» (02:41–02:50).** El informe cubre monto (RF07) y factor (RF06). Al revisar el Excel (A3), la carga masiva de montos es justamente la de la **DJ 1948** («Carga de archivo calificaciones masivas (Montos – DJ1948)», hoja *Objetivo y alcance*, A20; y A42 «carga externa de la DJ 1948»). Es decir, la entrada «desde la DJ» sí está cubierta por RF07/HU05, **pero el informe no lo dice con esas palabras** (D03 menciona la DJ1948 solo para fijar el año). *Corrijo así lo que había escrito antes: no es un requisito faltante, es una relación que conviene dejar explícita.* Sigue pendiente confirmar si el cliente espera otro modo de entrada directo desde el PDF de la DJ.
2. **«Anual» frente a «constante».** El informe presenta «actualización anual» como petición del cliente (sección 11). En el video, el proceso tributario es anual y el almacenamiento es anual, pero lo que se pide es «actualización constante» (01:14–01:20) y gestión «durante todo el año» (00:18–00:35). Conviene ajustar el texto.
3. **Frecuencia de carga.** Los emisores informan **una vez al año** (02:08–02:16). Eso sugiere cargas masivas estacionales, relevante para volúmenes y para RNF04. El informe no lo menciona.
4. **Roles.** El video habla de «corredores» como usuarios. El supervisor, el auditor y el administrador son una **propuesta del equipo**, no del video; el informe los lista como «actores» sin marcarlo.
5. **Quién habla.** Se presenta como «Especialista de Proyectos de Implementación en Nuam» (00:08–00:13). El informe lo nombra («Eduardo Leiva») pero no registra su cargo. La ortografía **Leiva** queda confirmada por el Excel: hoja *Control de Versiones*, Autor = «Eduardo Leiva Palomera», Empresa solicitante = «nuam». Whisper escribió «Leyva» y «Noam», que son errores de reconocimiento.

## 3. Lo que el informe afirma y el video **no** respalda
Estos puntos vienen del HDU [A3], de la clase o son inferencias del equipo. El informe los marca como tales en general, pero conviene no atribuirlos a V2:
- Aislamiento entre corredoras y precedencia local sobre Bolsa.
- Versionado de reglas por ejercicio; instrumentos no inscritos; baja lógica.
- Contradicciones de fórmulas (D01–D11): son del Excel.
- Metas numéricas de RNF04 y RNF05.

## 4. Marcas de tiempo de V2 en el informe (no se cambiaron)
| Cita en el informe | Contenido citado | Lo que muestra la transcripción | Observación |
|---|---|---|---|
| `V2, 00:25–00:43` | Información manual desde distintas fuentes | 00:29–00:45 | Calza (±2 s) |
| `V2, 00:25–01:40` | Manejo manual, fuentes, funcionalidades | 00:29–01:45 | Calza |
| `V2, 01:01–01:40` | Validar, actualizar, identificar origen | 01:00–01:20 y 01:33–01:45 | Calza |
| `V2, 01:40–02:42` | Actores, SII, emisores | 01:40–01:49 es el cierre de la presentación; el tema empieza en **01:56** y llega a ~02:50 | **Inconsistente al inicio.** Sugerido: 01:56–02:50 |
| `V2, 02:42–03:02` | Certificados PDF sin formato uniforme | Certificados/PDF: **02:54–03:03** | Empieza antes de lo citado. Sugerido: 02:54–03:03 |
| `V2, 02:42–03:33` | PDF no uniformes y años anteriores | 02:54–03:36 | El final cortaba la última frase (termina 03:36) |
| `V2, 03:02–03:33` | Recuperar DJ de años anteriores | 03:03–03:36 | Igual: sugerido 03:03–03:36 |
| `Vimeo, 03:45` | Duración | 03:44 (224,6 s) | Calza |

## 4b. Frente al Excel HDU_Inacap (A3): verificación de las citas del informe
Revisé las 8 hojas del archivo `HDU_Inacap (2).xlsx` y comprobé las citas que el informe hace a A3.

| Cita del informe | Qué dice el Excel | Resultado |
|---|---|---|
| HU01 «A3, filas 5/15» | Fila 5 = Mantenedor (filtros, grilla); fila 15 = columna de fuente de ingreso | Calza |
| HU02 «filas 6–8», HU03 «fila 9», HU04 «fila 10», HU05 «filas 11–14» | 6 Ingreso de calificación; 7 montos; 8 Calcular; 9 factores; 10 Modificar/eliminar; 11–14 cargas masivas y archivo | Calza |
| D01 «K8/K9; Flujo A19: suma 8–16 frente a 8–19» | K8 y K9: «suma del factor 8 al 16 no debe superar 1»; Flujo A19: «suma de los factores del 8 al 19 ≤ 1» | **Confirmada la contradicción** |
| D02 «29 campos frente a 30 códigos entre 8 y 37» | K7: «29 campos»; hoja Archivo: Factor 8 … Factor 37 (30 filas) | Confirmada |
| D03 «DJ1948, DJ1949, DJ1922 y certificados 70/44» | Homologación: «Cert 70 / 1948» y «Certificado 44 / 1922»; Tipos: «DJ 1949» | Confirmada |
| D05 «E21 remite a Q9; la secuencia sugiere T9» | Tipos: E21 → `Q9` y E22 → `U9` (salta de Q a U) | Consistente con lo observado (no verifiqué toda la columna) |
| D06 «largo 9 y un entero/ocho decimales» | Archivo: Largo 9; «1 entero, 8 decimales» | Confirmada |
| D07 «formato de fecha distinto del ejemplo» | Archivo: formato `DD-MM-AAAA`; ejemplo `2023-12-12` | Confirmada |
| D08 «K14, clave no definida» | K14: «Se debe considerar una llave para actualizar» | Confirmada |
| D09 «K6, rango de secuencia» | K6: «secuencia evento superior a los 10.000» | Confirmada |
| D11 «K12 repite factores» | K12: contexto y evento copiados de la fila de factores | Confirmada |
| «Precedencia local», «log», «ingreso por distintos orígenes» | Hoja *Objetivo y alcance* A37–A43 | Calza |

**Cosas del Excel que el informe no recoge o que conviene avisar:**
- A43 dice que el log «está detallado al final del HDU», pero **ese detalle no existe en el archivo** (la última hoja es *Flujo de proceso*). Es una consulta más para el cliente.
- La sección **Restricciones** (A29–A35) está **vacía**, y *Control de Versiones* tiene Fecha y Versión sin completar. Sirve para la Actividad 1 de la guía (restricciones administrativas): hoy no hay datos del cliente.
- En la hoja de historias, el número de escenario se repite (el **9** aparece dos veces: filas 12 y 13) y el 8 está después del 5; no afecta al informe, pero el equipo debe tener cuidado si cita «escenario N».
- El Excel sí marca el proyecto como **CORE**.

## 5. Frente a la guía (¿lo que pide el video está cubierto por lo que pide la guía?)
- El video pide **analizar requerimientos, identificar riesgos y proponer un diseño técnico**: la guía lo bajó a RF/RNF, HU, metodologías y seguridad. El informe cubre las cuatro actividades.
- La guía espera además que el equipo haga **su propio levantamiento** (entrevistas, encuestas, observación). El informe trabaja solo con las entrevistas aportadas y declara las demás como pendientes: está bien explicado, pero es el punto más débil frente a la Actividad 2.

## 6. Frente a la rúbrica (criterios 1.1.1–1.1.5)
Los cinco criterios están cubiertos por alguna sección. Lo débil es el detalle: ver el listado en `pendientes_equipo.md` (sección B).
