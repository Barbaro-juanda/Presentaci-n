# SUSI 2030 · Informe de prospectiva estratégica

Presentación final de **Prospectiva 1** (ESIC, Digital Business & Administration) sobre
**SUSI S.A.S.**, panadería y repostería artesanal.

- **Equipo:** Juan David Escobar Guiral · Santiago Duque Restrepo · María Camila Jiménez Ramírez · Thomas Quintero Gallego
- **Profesor:** Carlos Alberto Rincón
- **Fecha:** 30 de septiembre de 2026
- **Duración objetivo:** 12–15 minutos hablados · 18 diapositivas

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
8. Validación con experta
9. Qué cambió por la validación
10. Tres futuros posibles
11. Optimista · «El pan que se deja leer»
12. Pesimista · «La góndola sin nombre»
13. Tendencial · «Buen pan, poca voz»
14. Hoja de ruta 2026–2030
15. Recomendaciones 1 a 4
16. Recomendaciones 5 a 8
17. Los próximos seis meses
18. Referencias (APA 7)

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

Todo el contenido proviene del informe `Informe_prospectiva_SUSI_APA7_12p`. No se
añadieron cifras, citas ni datos que no estén en él. Las dos metas marcadas con la
etiqueta punteada **«Meta propuesta por el equipo»** (recomendaciones 7 y 8) se señalan
así porque son estimaciones nuestras y no cifras del informe.
