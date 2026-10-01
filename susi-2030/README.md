# SUSI 2030 · Informe de prospectiva estratégica

Presentación final de **Prospectiva 1** (ESIC, Digital Business & Administration) sobre
**SUSI S.A.S.**, panadería y repostería artesanal.

- **Equipo:** Juan David Escobar Guiral · Santiago Duque Restrepo · María Camila Jiménez Ramírez · Thomas Quintero Gallego
- **Profesor:** Carlos Alberto Rincón
- **Fecha:** 30 de septiembre de 2026
- **Duración objetivo:** 12–15 minutos hablados · 19 diapositivas

## Cómo se abre

`index.html` es un único archivo autónomo: no necesita servidor, ni conexión, ni CDN.
Las fuentes (Space Grotesk y JetBrains Mono) y GSAP 3.12.5 van incrustados en el propio
archivo, y además quedan como copia legible en `fonts/` y `vendor/`.

## Navegación

| Tecla | Acción |
|---|---|
| `→` `↓` `espacio` · clic | Avanzar una diapositiva |
| `←` `↑` | Retroceder |
| `Inicio` · `Fin` | Primera y última |
| `P` | Modo presentación (oculta el portal y entra a pantalla completa) |
| `O` | Cuadrícula de diapositivas |
| `N` | Guion del expositor |
| `T` · `R` | Cronómetro: iniciar/pausar · reiniciar |
| `F` | Pantalla completa |
| `Esc` | Cerrar lo que esté abierto |

**Una diapositiva por clic.** No hay sub-pasos: cada clic avanza una lámina completa.

## Estructura

1. Portada
2. El reto en una frase
3. Quién es SUSI
4. Macroentorno
5. Microentorno · cinco fuerzas de Porter
6. Seis variables críticas (MICMAC)
7. Cómo construimos los escenarios
8. Las seis hipótesis (H1 a H6)
9. Validación con experta
10. Qué cambió por la validación
11. Tres futuros posibles
12. Optimista · «El pan que se deja leer»
13. Pesimista · «La góndola sin nombre»
14. Tendencial · «Buen pan, poca voz»
15. Hoja de ruta 2026–2030
16. Recomendaciones 1 a 3
17. Recomendaciones 4 a 6
18. Los próximos seis meses
19. Cierre y normativa citada

## Dirección de arte

- Paleta SUSI **sin alterar**: `#D83624`, `#B41212`, `#C06030`, `#B05030`, `#EA4836`,
  `#1A1A1A`, `#D8D8D8`, `#F7F3EC`. El registro oscuro se construye con derivados de
  opacidad sobre `--crema`, no con colores nuevos.
- Futurismo sobrio: fondo profundo, rejilla HUD con máscara radial, halos cálidos de la
  propia paleta, tarjetas de vidrio y grano sutil. Sin neón, sin azules de ciencia ficción.
- Space Grotesk (geométrica moderna) para títulos y cifras; JetBrains Mono para etiquetas,
  números técnicos y la interfaz.
- **Hilo conductor:** la línea de tiempo 2026 → 2030 al pie de todas las diapositivas avanza
  según la etapa del argumento.
- Animación con GSAP: solo `opacity`, `transform` y `scaleX`. Respeta
  `prefers-reduced-motion`, y sin JavaScript el contenido se ve completo y estático.

## Fuente del contenido

Todo el contenido proviene de **`Informe de prospectiva estratégica Grupo 2.docx`**, el
informe final. No se añadieron cifras, citas ni datos que no estén en él.

**Pendientes y contradicciones del informe, señalados en el deck:**

1. El informe final **no incluye lista de referencias en APA 7**. La lámina 19 muestra la
   normativa citada dentro del texto y marca el faltante con la etiqueta «Pendiente».
2. El **resumen ejecutivo** nombra como variables críticas «sellos, innovación, costos,
   cadenas, impuesto y nostalgia», mientras la **sección 2.3** define V1 Innovar, V2 Costos,
   V3 Cadenas, V4 Competir, V5 Alianzas y V6 Digital. El deck usa las de la sección 2.3,
   que es el análisis MICMAC formal; las recomendaciones conservan los nombres con los que
   el informe las etiqueta.
3. La **sección 3.2** dice que se sumaron dos recomendaciones (panadería-laboratorio e
   inteligencia artificial), pero la **sección 5 solo lista seis** y ninguna es esa. El deck
   sigue la sección 5.
4. El informe **nombra H1 a H6 sin transcribir su enunciado**. Los textos de la lámina 8
   están redactados por el equipo a partir de los tres relatos de escenario, y la lámina lo
   declara al pie.
5. El informe escribe el nombre de la panadería de la experta como «Pané». El nombre correcto
   es **Panem**, y así aparece en el deck. Hay que corregirlo en el informe.

**Las seis hipótesis.** El informe nombra H1 a H6 y las empareja con cada escenario, pero no
transcribe su enunciado: solo desarrolla los tres relatos. Los textos de la lámina 8 están
redactados por el equipo a partir de esos relatos, sin añadir nada que no esté en el informe,
y la lámina lo declara al pie.
