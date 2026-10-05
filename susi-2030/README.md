# SUSI 2030 · Informe de prospectiva estratégica

Presentación final de **Prospectiva 1** (ESIC, Digital Business & Administration) sobre
**SUSI S.A.S.**, panadería y repostería artesanal.

- **Equipo:** Juan David Escobar Guiral · Santiago Duque Restrepo · María Camila Jiménez Ramírez · Thomas Quintero Gallego
- **Profesor:** Carlos Alberto Rincón
- **Fecha:** 30 de septiembre de 2026
- **Duración objetivo:** 15 minutos hablados · 21 diapositivas

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
16. Recomendaciones 1 y 2
17. Recomendaciones 3 y 4
18. Recomendaciones 5 y 6
19. Recomendaciones 7 y 8
20. Los próximos seis meses
21. Cierre y normativa citada

## Dirección de arte

**Brutalismo técnico sobre el esquema del empaque.** Dos registros intercalados:
**oscuras** en portada, «El reto», «Tres futuros», «Los próximos seis meses» y el
cierre —fondo `#16130F`, texto `#F2E7D4`, brasa `#F0A23C`, crítico `#EC6A3A`—; y
**claras** en todas las de datos —kraft `#F3E9D6`, tinta `#201A12`, ladrillo
`#B23A28`, ámbar `#C7601E`—. Ladrillo, ámbar, negro y crema: nada de azul.

**Tipografía:** Saira Condensed itálica 700 para titulares y cifras, Inter para
cuerpo, Space Mono para el HUD.

**Kit HUD:** miras en las cuatro esquinas, etiqueta de marca, etiqueta de lámina
que se tipea con cursor, asteriscos, timestamp vivo, anillos que giran y banda
tipo ticket arriba y abajo, que es el motivo del toldo del empaque.

**Las imágenes son planos vivos.** Duotono ámbar/charcoal por CSS, Ken Burns
continuo de 13 s, barrido de luz en bucle lento, reveal cinemático con máscara
`clip-path` al entrar la lámina, y la espiga que se mece. Solo en portada,
divisores y cierre; las láminas de datos van limpias.

**Chispas de brasa** en canvas sobre las láminas oscuras: 26 partículas, solo
transform, se apagan al pasar a una lámina clara. Grano de papel sembrado que
tiembla en pasos. Glitch de scanline brevísimo solo entre dos láminas oscuras.

**Profundidad.** Cada lámina es una escena de tres planos —fondo a −640 px,
contenido a 0, borde a +170— inyectados sin tocar el marcado. Al entrar, el plano
lejano llega lento y desenfocado; el cursor inclina el mundo unos grados con
amortiguación.

**Los datos nunca se vuelven ilegibles.** Las barras crecen desde su eje, las seis
variables del plano aterrizan con pulso —ámbar las que SUSI controla, terracota
las críticas— y una línea de escaneo cruza el bloque una sola vez al entrar.
Solo se animan `transform` y `opacity`. Con `prefers-reduced-motion` se apagan
Ken Burns, chispas, glitch y parallax, y quedan fundidos simples.

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
   presenta las ocho: las seis de la sección 5 del informe final y las dos adicionales con
   el texto del informe anterior, marcadas con la etiqueta «Meta propuesta por el equipo».
   **Hay que agregar esas dos fichas a la sección 5 del informe** para que documento y
   presentación coincidan.
4. El informe **nombra H1 a H6 sin transcribir su enunciado**. Los textos de la lámina 8
   están redactados por el equipo a partir de los tres relatos de escenario, y la lámina lo
   declara al pie.
5. El informe escribe el nombre de la panadería de la experta como «Pané». El nombre correcto
   es **Panem**, y así aparece en el deck. Hay que corregirlo en el informe.
6. En la recomendación 3 el informe propone «harinas de yuca o cereales ancestrales». El deck
   las reemplaza por **plátano verde, leguminosas y salvado de avena**, más fermentación larga
   con masa madre, porque son las que de verdad bajan el índice glucémico. Hay que actualizarlo
   en el informe.
7. La recomendación 7 pasa de 9 meses a un horizonte de **3 a 4 años** por decisión del equipo.
   El informe anterior decía 9 meses.

**Las seis hipótesis.** El informe nombra H1 a H6 y las empareja con cada escenario, pero no
transcribe su enunciado: solo desarrolla los tres relatos. Los textos de la lámina 8 están
redactados por el equipo a partir de esos relatos, sin añadir nada que no esté en el informe,
y la lámina lo declara al pie.
