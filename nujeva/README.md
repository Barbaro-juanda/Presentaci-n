# NUJEVA · Análisis de mercado y redefinición del buyer persona

Presentación web de 20 escenas para sustentar el documento de trabajo
*Informe Buyer Persona Nujeva (actualizado)*. Todo el contenido —cifras, citas,
segmentos, objeciones, journey, universo temático y referencias— sale de ese PDF;
no hay dato, competidor, certificación ni registro añadido.

## Cómo abrirla

Doble clic en `index.html`. No necesita servidor, internet ni instalación.
GSAP, ScrollTrigger y las tres tipografías viajan dentro del archivo.

## Navegación · el mismo portal que las demás presentaciones

Barra superior con cronómetro y botones, panel lateral con las veinte escenas en
miniatura real, y el lienzo de 1920×1080 escalado al centro. **Presentar** oculta
todo el chrome y entra en pantalla completa. Ya no se navega por scroll: cada
escena ocupa el lienzo completo y se avanza de una en una.

| Tecla | Acción |
|---|---|
| `→` `↓` `espacio` · clic | Escena siguiente |
| `←` `↑` | Escena anterior |
| `Inicio` · `Fin` | Primera · última |
| `P` | Modo presentación |
| `O` | Vista de cuadrícula con las 20 escenas |
| `N` | Notas del orador (dos frases guía por escena) |
| `T` | Cronómetro 00:00 → 10:00 |
| `F` | Pantalla completa |
| `R` | Reinicia el cronómetro |
| `Esc` | Cierra lo que esté abierto |

La rueda del ratón también avanza de escena en escena. Los elementos
interactivos —los nodos del ecosistema, las objeciones desplegables y el
recorrido de nueve etapas— siguen respondiendo al ratón sin hacer avanzar la
presentación.

## Etiquetas epistemológicas

Cada bloque indica de qué tipo es la afirmación, con color **y** forma distintos:

| Etiqueta | Forma | Significa |
|---|---|---|
| DATO | cuadrado | Cifra de fuente secundaria, siempre con su referencia `[n]` |
| HALLAZGO | círculo | Lectura que el informe da por establecida |
| INTERPRETACIÓN | rombo | Lectura estratégica del equipo |
| HIPÓTESIS | triángulo + borde punteado | **No validado.** Requiere investigación primaria |
| OPORTUNIDAD | chevron | Implicación accionable |

Las hipótesis nunca se presentan como validadas, y los territorios de mensaje
aparecen marcados como rutas creativas preliminares, no como claims.

## Estructura de archivos

```
nujeva/
├── index.html      la presentación completa y autocontenida
├── fonts/          Fraunces · Inter · JetBrains Mono (.woff2, licencia abierta)
├── vendor/         GSAP 3.12.5 y ScrollTrigger, servidos en local
└── README.md
```

`index.html` incrusta esos mismos archivos en base64, así que funciona aunque se
mueva solo. Las carpetas quedan como fuente y atribución.

## Encapsulado

Todo el CSS vive bajo `#nj` y con prefijo `.nj-`, y las tipografías se registran
con nombres propios (`NJ Serif`, `NJ Sans`, `NJ Mono`). Nada de esta carpeta
afecta a las demás presentaciones del repositorio.

## Accesibilidad y rendimiento

- Respeta `prefers-reduced-motion`: sin animación, todo visible.
- Si el JavaScript falla, `#nj` conserva la clase `.nj-no-js` y el contenido
  completo queda legible.
- Solo se animan `opacity`, `transform` y `stroke-dashoffset`.
- El lienzo mide siempre 1920×1080 y se escala a la ventana, así que la
  composición es idéntica en cualquier resolución. Sin desbordes ni scroll.

## Nota de contenido

El informe distingue entre dato secundario, interpretación e hipótesis. Dos
puntos que conviene repetir en voz alta al presentar:

- El **21,3 %** de Belén es la caracterización del Plan de Desarrollo Local de la
  Comuna 16, no una medición de 2026.
- Los perfiles de **Laureles–Estadio** son contextuales por la antigüedad de las
  fichas; no son una fotografía socioeconómica actual.
