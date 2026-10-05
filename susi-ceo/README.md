# SUSI 2030 · Síntesis ejecutiva para la CEO

Las tres entregas de Prospectiva 1 fundidas en una sola historia de **10 minutos**,
dirigida a Susanne Seifert, dirección general de SUSI Panadería Artesanal.

## Qué trae de cada entrega

| Entrega | Qué sobrevive aquí |
|---|---|
| **1 · Análisis del entorno** | La tesis: 12 de los 15 puntos de contacto son de terceros. El precio, 3,58× el promedio masivo. Porter. |
| **2 · MICMAC** | El método en una lámina: 20 variables → 400 cruces → 6 palancas, con la estabilidad al 100 %. |
| **3 · Informe final** | Casi todo lo demás: las seis palancas, los tres escenarios, la hoja de ruta y las ocho decisiones con plazo e impacto. |

La prioridad es la entrega 3, como se pidió: siete de las doce láminas salen de ahí.

## Cómo se abre

`index.html` es un archivo único y autónomo: sin servidor, sin conexión, sin CDN.
Fuentes y GSAP van incrustados, y quedan además como copia legible en `fonts/` y `vendor/`.

## Navegación

| Tecla | Acción |
|---|---|
| `→` `↓` `espacio` · clic | Avanzar |
| `←` `↑` | Retroceder |
| `Inicio` · `Fin` | Primera y última |
| `P` | Modo presentación |
| `O` | Cuadrícula |
| `N` | Guion |
| `T` · `R` | Cronómetro: iniciar/pausar · reiniciar |
| `F` | Pantalla completa |
| `Esc` | Cerrar |

## Expositores

María Camila Jiménez Ramírez · Santiago Duque Restrepo · Juan David Escobar Guiral.
Cada lámina lleva en `data-quien` quién la dice, y el guion abre con el reparto.

## Dirección de arte

**Papel, ámbar líder, rojo mínimo.** Fondo `#FAF3E4`, tinta `#201A12`, ámbar de
sistema `#E0912B` (profundo `#B9711A`). El terracota `#B23A28` queda reservado a
las variables críticas y al hallazgo principal; el azul marino `#223B5B` tiene un
solo uso, lo estructural y el futuro. Banda superior tipo ticket con franjas
verticales crema/ámbar, como el toldo del empaque.

**Datos.** Matriz 20 × 20 en escala de calor crema → ámbar → tinta, con terracota
solo en el cruce más fuerte, rotulado para que no dependa del color. La paleta de
marcas (`#E0912B`, `#B23A28`, `#3A6FA5`) pasa las seis comprobaciones del
validador: banda de luminosidad, piso de croma, separación para daltonismo,
piso de visión normal y contraste. El azul de marcas es un paso más claro que el
azul estructural, porque el original no alcanzaba el piso de croma.

**Movimiento: profundidad.** Cada lámina es una escena con capas a distinta
distancia de la cámara. Al entrar, el plano más lejano llega lento y desenfocado,
y los cercanos llegan antes: la sensación es de cámara que avanza. El cursor
inclina el mundo unos pocos grados, con amortiguación. Los datos nunca se mueven
hasta volverse ilegibles: las barras crecen desde su eje y las 400 celdas solo
aparecen en barrido. Solo se animan `transform`, `opacity` y `filter`.

**Grano de papel generativo.** El fondo no es una foto: es ruido sembrado
dibujado una vez en un canvas, con fibra de baja amplitud y motas ocasionales.
Mismo resultado en cada apertura, coste cero por cuadro.

**Imágenes.** El logotipo y la espiga de trigo son vectores dentro del archivo.
`img/textura-kraft.jpg` y `img/grabado-horno.png` son opcionales: si faltan, ese
plano de profundidad no se dibuja y el resto queda intacto.

**Tipografía:** Fraunces para titulares y cifras, Inter para cuerpo, JetBrains
Mono para datos y etiquetas.

## Diferencias con el deck académico

Esta versión habla a una CEO, no a un jurado. No defiende el método: lo nombra en
una lámina y sigue. No muestra hipótesis ni validación con expertos. Y cierra
pidiendo una decisión concreta sobre tres acciones del trimestre, no resumiendo.
