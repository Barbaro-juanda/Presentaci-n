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

**Los colores salen de los empaques,** muestreados de las fotos de producto
(solo la paleta: el deck no usa fotografías):
el naranja `#E43018` de las bolsas «70 % menos azúcar», el azul `#0078CC` de la
banda, el ámbar `#E4A80C` del arroz soplado y el kraft del cereal.

**Cinco registros, cada uno atado a una función del relato,** para que el deck
respire en lugar de ser un solo bloque de color:

| Registro | Fondo | Para qué |
|---|---|---|
| `r-papel` | kraft cálido | quiénes somos, la marca, los escenarios |
| `r-claro` | casi blanco | los datos y el método |
| `r-sello` | negro | la tensión: el costo y el escenario que preocupa |
| `r-senal` | azul profundo | la acción: lo que pedimos |
| `r-marca` | rojo SUSI | el cierre |

**Tipografía:** Fraunces (serif con carácter) para los titulares y las cifras,
porque el logotipo de SUSI es serif y la marca es de oficio; Inter para el cuerpo;
JetBrains Mono para datos y etiquetas.

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
