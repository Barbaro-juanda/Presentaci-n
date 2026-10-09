# Chickenmart conectado · Pitch ejecutivo final

Presentación final del proyecto académico de **transformación digital para Chickenmart S.A.S.**
(Alto de Las Palmas, Envigado). Es la exposición completa del equipo y cierra pidiendo una
decisión de inversión defendida con problema, evidencia, viabilidad y resultado.

- **Lema:** «Chickenmart conectado: del peso recibido a la disponibilidad de venta».
- **Equipo, en orden de exposición:** Santiago → Juan David → Carolina → Nataly → Orozco.
- **Duración:** 16 diapositivas · ~13:35 hablados · cronómetro a 15:00.
- **Guion completo** (título, contenido, visual y notas por diapositiva): `guion.md`.

## Cómo se abre

`index.html` es un único archivo autónomo: no necesita servidor, conexión ni CDN. Nunito,
Inter, Space Mono y GSAP 3.12.5 van incrustados en el propio archivo, y además quedan como
copia legible en `fonts/` y `vendor/`.

## Navegación · el mismo portal que las demás presentaciones

| Tecla | Acción |
|---|---|
| `→` `↓` `espacio` · clic | Avanzar una diapositiva |
| `←` `↑` | Retroceder |
| `Inicio` · `Fin` | Primera y última |
| `P` | Modo presentación (oculta el portal y entra a pantalla completa) |
| `O` | Cuadrícula de diapositivas |
| `N` | Guion del expositor (con número, quién expone y segundos) |
| `T` · `R` | Cronómetro: iniciar/pausar · reiniciar |
| `F` | Pantalla completa |
| `Esc` | Cerrar lo que esté abierto |

**Una diapositiva por clic.** Cada escena entra completa con su coreografía; no hay
sub-pasos. Se puede abrir directo en una lámina con `index.html#11`.

## Reparto

| Expositor | Diapositivas | Tiempo |
|---|---|---|
| Santiago | 1 Portada · 2 Problema · 3 AS IS → TO BE · 16 (mitad) | 2:50 |
| Juan David | 4 Arquitectura e IoT · 5 Automatizaciones · 16 (mitad) | 2:30 |
| Carolina | 6 Cloud · 7 IA · 14 Costos, KPIs y ROI | 2:40 |
| Nataly | 8 Agentes · 12 Roadmap · 13 Riesgos · coordina la 11 | 2:20 + demo |
| Orozco | 9 Data Hub y Power BI · 10 Gemelo digital · 15 Industria 5.0 | 2:15 |

En escena, el HUD de abajo dice siempre quién expone (`EXPONE // NATALY`) y el panel de
miniaturas marca las láminas pendientes. Cada cambio de expositor tiene su frase de relevo en
las notas (`RELEVO →`).

## Reglas de contenido

- **No hay datos inventados.** No se usan ventas, costos, ahorros, número de empleados ni
  plataformas. Todo número de ejemplo lleva la marca **✳ ficticio** o **✳ supuesto**
  (21,62 − 1,62 = 20,00 kg; 20 − 4 − 1 = 15 kg; 8–12 semanas).
- **Nada de lo propuesto está instalado hoy en Chickenmart.** La portada lo dice y la demo lo
  repite para el prototipo.
- Los gráficos de IA (lámina 7) son ilustrativos y lo declaran en pantalla.
- La matriz de riesgos muestra la escala, pero no ubica ningún riesgo: eso es de Nataly.

### Etiquetas · color y forma, nunca solo color

| Etiqueta | Forma | Significa |
|---|---|---|
| HECHO | cuadrado lleno, borde sólido, en tinta | Sale del diagnóstico |
| PROPUESTA | círculo, en el acento de la marca | Lo propone el equipo |
| PENDIENTE | triángulo, borde punteado y rayado de obra | Falta contenido o validación |
| ✳ FICTICIO · SUPUESTO | asterisco subrayado | Número de ejemplo, no real |

## Láminas pendientes

Se diseñaron con estructura, títulos y un recuadro visible «Contenido pendiente de [nombre]»
con cinta de obra animada:

| Lámina | Quién | Qué falta |
|---|---|---|
| 8 Agentes G1–G3 | Nataly | Objetivo final, quién aprueba en G2 y G3, evidencia |
| 9 Data Hub y Power BI | Orozco | Modelo final y captura del tablero (datos ficticios del prototipo) |
| 10 Gemelo digital | Orozco | Base, cambio, resultado y decisión de los tres escenarios |
| 11 Demo integrada | Carolina, Nataly, Orozco | Evidencias de IA, agentes, tablero y gemelo |
| 12 Roadmap | Nataly | Duración, responsables y entregable de cada fase |
| 13 Riesgos | Nataly | Ubicación de R1–R9 en la matriz |
| 15 Industria 5.0 | Orozco | Desarrollo final de pilares y visión |

Cuando llegue el contenido: se borra el `.pend-box`, se quita `data-pend="1"` de la
`<section>` y la etiqueta `tag pend` del encabezado, y se reemplaza el `[PENDIENTE …]` de
las notas (`data-n`).

## Sobre los 18 criterios de la rúbrica

La rúbrica no está en el repositorio, así que no se pudo cruzar criterio por criterio. La
estructura cubre: problema, diagnóstico, AS IS / TO BE, arquitectura, IoT, automatizaciones,
cloud, IA, agentes, Data Hub y Power BI, gemelo digital, implementación (demo), roadmap,
riesgos, costos, KPIs, ROI e Industria 5.0 con visión, y cierra con la decisión. **Conviene
revisarla contra la rúbrica oficial** antes de exponer.

## Dirección de arte

Misma infraestructura que `susi-2030` —portal, cámara en tres planos, kit HUD, malla de
color, sello extruido— con la identidad de Chicken Mart.

**Paleta de la marca:** vino `#7D0608` (principal), crema `#FFE6C1`, casi negro `#070A11`
(texto) y blanco hueso `#FCF7F5` (fondo). Para legibilidad se derivan dos tonos: un vino claro
`#FF8E92` para texto sobre negro (8,99:1) y un dorado de fritura `#94550A` para alertas sobre
hueso (5,55:1). Todos los pares de texto superan 4,5:1.

**Tres registros:** siete oscuras (portada, problema, arquitectura, cloud, agentes, gemelo,
Industria 5.0), ocho claras para lo más denso de leer, y una vino reservada a la decisión.

**Tipografía:** Nunito 900 para titulares y cifras (robusta, de trazos suaves), Inter para
el cuerpo y Space Mono para el HUD, etiquetas y lecturas de báscula.

**Marca:** el logo es un **redibujo de trabajo** —la cabeza del gallo integrada a la «C»—
definido una sola vez como `<symbol id="cm-logo">`. Para usar el logo oficial basta con
reemplazar el contenido de ese símbolo (y la constante `LOGO` del script, que alimenta la
máscara del lustre).

**Motivos propios:** la banda superior es la **regla graduada de una báscula**; el dial de la
esquina gira como un indicador de peso; en las oscuras suben **bits de datos** crema en lugar
de chispas; el riel inferior avanza por capítulos (diagnóstico → solución → inteligencia →
ejecución → decisión).

**Motion graphics, lámina por lámina:** el lema se arma letra por letra; las agujas de los
medidores caen con rebote; el TO BE se dibuja y un pulso lo recorre en bucle mientras el paso
«después» del AS IS tiembla; los cables de la arquitectura se trazan y los paquetes viajan en
los dos sentidos; la báscula cuenta hasta 20,00 kg y la barra apilada se reparte; la IA dibuja
su banda de incertidumbre y enciende el punto raro; los esqueletos «cargan» en lo pendiente;
los riesgos caen con rebote a su bandeja; y en el cierre la pila se construye desde la base.
Solo se animan `transform`, `opacity`, `clip-path` y filtros. Con `prefers-reduced-motion`
todo queda quieto y visible.
