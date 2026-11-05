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
1. **Tres modos de entrada, no dos.** El video dice que se requiere cargar «por monto, por factor o directamente de una declaración jurada» (02:41–02:50). El informe cubre monto (RF07) y factor (RF06), y vincula fuentes (RF12), pero **no tiene un RF/HU para ingresar directamente desde una DJ**. Hay que confirmar con la contraparte si es un requisito.
2. **«Anual» frente a «constante».** El informe presenta «actualización anual» como petición del cliente (sección 11). En el video, el proceso tributario es anual y el almacenamiento es anual, pero lo que se pide es «actualización constante» (01:14–01:20) y gestión «durante todo el año» (00:18–00:35). Conviene ajustar el texto.
3. **Frecuencia de carga.** Los emisores informan **una vez al año** (02:08–02:16). Eso sugiere cargas masivas estacionales, relevante para volúmenes y para RNF04. El informe no lo menciona.
4. **Roles.** El video habla de «corredores» como usuarios. El supervisor, el auditor y el administrador son una **propuesta del equipo**, no del video; el informe los lista como «actores» sin marcarlo.
5. **Quién habla.** Se presenta como «Especialista de Proyectos de Implementación en Nuam» (00:08–00:13). El informe lo nombra («Eduardo Leiva») pero no registra su cargo. Verificar la ortografía del apellido (el archivo dice *Leiva*; Whisper escribió *Leyva*).

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

## 5. Frente a la guía (¿lo que pide el video está cubierto por lo que pide la guía?)
- El video pide **analizar requerimientos, identificar riesgos y proponer un diseño técnico**: la guía lo bajó a RF/RNF, HU, metodologías y seguridad. El informe cubre las cuatro actividades.
- La guía espera además que el equipo haga **su propio levantamiento** (entrevistas, encuestas, observación). El informe trabaja solo con las entrevistas aportadas y declara las demás como pendientes: está bien explicado, pero es el punto más débil frente a la Actividad 2.

## 6. Frente a la rúbrica (criterios 1.1.1–1.1.5)
Los cinco criterios están cubiertos por alguna sección. Lo débil es el detalle: ver el listado en `pendientes_equipo.md` (sección B).
