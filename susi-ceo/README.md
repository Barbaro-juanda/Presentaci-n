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

## Dirección de arte

Paleta SUSI intacta sobre negro pleno, en continuidad con la entrega 3.
El riesgo se gasta entero en el movimiento, no en cambiar la identidad.

**El ensamblaje.** Cada cifra y cada titular se arma solo: las letras entran desde
posiciones dispersas en el espacio 3D, desenfocadas, se pasan de largo y encajan.
Viene del reveal de logo que sirvió de referencia.

**El anillo de dependencia.** En la lámina 2, quince puntos orbitan el núcleo de la
marca; luego doce se desprenden hacia afuera del aro. La tesis hecha literal, no
ilustrada. Es el elemento por el que se recuerda el deck.

Solo se animan `opacity`, `transform` y `filter`. Respeta `prefers-reduced-motion`
y, sin JavaScript, el contenido se ve completo y estático.

## Diferencias con el deck académico

Esta versión habla a una CEO, no a un jurado. No defiende el método: lo nombra en
una lámina y sigue. No muestra hipótesis ni validación con expertos. Y cierra
pidiendo una decisión concreta sobre tres acciones del trimestre, no resumiendo.
