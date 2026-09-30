# NUJEVA · Análisis de mercado y redefinición del buyer persona

Presentación web de 20 escenas para sustentar el documento de trabajo
*Informe Buyer Persona Nujeva (actualizado)*. Todo el contenido —cifras, citas,
segmentos, objeciones, journey, universo temático y referencias— sale de ese PDF;
no hay dato, competidor, certificación ni registro añadido.

## Cómo abrirla

Doble clic en `index.html`. No necesita servidor, internet ni instalación.
GSAP, ScrollTrigger y las tres tipografías viajan dentro del archivo.

## Navegación

| Tecla | Acción |
|---|---|
| `→` `↓` `espacio` | Escena siguiente |
| `←` `↑` | Escena anterior |
| `Inicio` · `Fin` | Primera · última |
| `I` | Índice de las 20 escenas |
| `Esc` | Cerrar el índice |

También funciona con scroll normal. Arriba a la derecha hay un contador `05 / 20`
y una barra de progreso en el borde superior.

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
- Probada sin desbordes ni scroll horizontal en 1920×1080, 1440×900 y 1366×768.

## Nota de contenido

El informe distingue entre dato secundario, interpretación e hipótesis. Dos
puntos que conviene repetir en voz alta al presentar:

- El **21,3 %** de Belén es la caracterización del Plan de Desarrollo Local de la
  Comuna 16, no una medición de 2026.
- Los perfiles de **Laureles–Estadio** son contextuales por la antigüedad de las
  fichas; no son una fotografía socioeconómica actual.
