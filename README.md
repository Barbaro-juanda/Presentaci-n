# Presentaciones de Prospectiva I — SUSI S.A.S.

Dos presentaciones autocontenidas en HTML para sustentar el trabajo de aplicación
de Prospectiva I sobre SUSI S.A.S. `index.html` es la portada que enlaza a ambas.

| Archivo | Entrega | Contenido |
|---|---|---|
| `SUSI-Prospectiva-2030.html` | 1 | Análisis del entorno, incidencia y favorabilidad |
| `SUSI-MICMAC-2030.html` | 2 | Análisis de impacto cruzado (MICMAC): matriz relacional, cuatro planos, desplazamientos y seis variables críticas |

Ambas comparten la misma infraestructura (panel de miniaturas, vista de cuadrícula, modo
presentación, notas del orador con `N`, cronómetro de 10 minutos) y los mismos atajos.

---

# Entrega 1 · Análisis del entorno, incidencia y favorabilidad

Presentación de prospectiva empresarial con horizonte **2030** sobre SUSI S.A.S.,
panadería artesanal y snacks saludables de Itagüí, Antioquia.

**Curso:** Prospectiva 1 · ESIC Business and Marketing School
**Docente:** Carlos Alberto Rincón
**Integrantes:** María Camila Jiménez Ramírez · Santiago Duque Restrepo · Juan David Escobar
**Retos trabajados:** Reto 1 «Las mezclas nostálgicas» · Reto 4 «Dónde están las oportunidades»

---

**En línea:** https://presentaci-n-five.vercel.app

## Cómo se abre

Descarga `SUSI-Prospectiva-2030.html` y ábrelo con doble clic en cualquier navegador.
Es **un solo archivo autocontenido**: no necesita internet, servidor, CDN ni dependencias.
El logo va incrustado como SVG dentro del propio HTML.

Diseñada para proyección **1920 × 1080 (16:9)**; el lienzo se escala solo a la ventana.

## Interfaz

Al abrir queda en modo edición/ensayo, con panel de miniaturas y barra superior.
El botón **Presentar** oculta todo el chrome y entra en pantalla completa.

| Tecla | Acción |
|---|---|
| `→` `Espacio` | Siguiente slide |
| `←` | Slide anterior |
| `Inicio` / `Fin` | Primero / último |
| `P` | Entrar o salir del modo presentación |
| `O` | Vista de cuadrícula con las 14 slides |
| `N` | Notas del orador |
| `F` | Pantalla completa |
| `R` | Reiniciar el cronómetro |
| `?` | Ayuda de atajos |

El cronómetro arranca en el **primer avance de slide** y marca el límite de 10:00.

## Contenido

14 slides. Reparto: María Camila 1–4 (3:00) · Juan David 5–9 (3:30) ·
Santiago 10–13 (3:00) · cierre 0:30.

1. Portada
2. El caso — SUSI en cuatro datos y los dos retos
3. Historia y portafolio
4. Canales actuales — 12 cadenas frente a 3 canales directos
5. Cinco fuerzas de Porter
6. Posición competitiva por precio
7. PESTEL hacia 2030
8. Tendencias micro · macro · mega
9. Implicaciones 2030 — tesis del trabajo
10. Las 20 variables críticas
11. Ejemplo de hipótesis a 2030
12. Plano de incidencia y favorabilidad
13. Síntesis por zonas
14. Cierre

## Cómo editar los datos

Los datos viven en arreglos al inicio del `<script>`, separados del diseño:

| Arreglo | Slide |
|---|---|
| `CADENAS` | 4 · cadenas del canal indirecto |
| `FUERZAS` | 5 · fuerzas de Porter e intensidad |
| `PRECIOS` | 6 · precio por 100 g |
| `PESTEL` | 7 · hallazgo por dimensión |
| `VARIABLES` | 10 y 12 · las 20 variables (`x` = favorabilidad, `y` = incidencia, 0–100) |

Cambiar una coordenada en `VARIABLES` mueve el punto en el plano y recalcula
solos los conteos por zona (liderazgo / crisis / ninguna).

## Diseño

Paleta e identidad tomadas del empaque real de SUSI: fondo crema, rojo del
empaque como acento, franjas rojas como motivo recurrente y el sello original
de la marca. Tipografía 100 % del sistema, sin fuentes externas: serif de alto
contraste (Didot / Bodoni) para títulos y sans humanista (Avenir / Segoe UI)
para el cuerpo.

Animaciones solo con `opacity`, `translate3d` y `scaleX`; respeta
`prefers-reduced-motion`.

---

# Entrega 2 · Análisis de impacto cruzado (MICMAC)

Archivo: `SUSI-MICMAC-2030.html`. Equipo 2: María Camila Jiménez Ramírez, Santiago Duque
Restrepo, Juan David Escobar y Thomas Quintero. Reparto: María Camila 1–4 (2:30) ·
Thomas 5–7 (2:25) · Juan David 8–10 (2:30) · Santiago 11–14 (2:35).

1. Portada
2. El método — de calificar variables a leer el sistema
3. Las 20 variables con nombre corto (V01–V20)
4. La matriz relacional 20 × 20 con los cinco cruces resaltados
5. Cinco cruces, cinco argumentos (uno por integrante + el colectivo)
6. Estabilidad de la matriz (convergencia por iteración)
7. Plano de influencias directas (MDI)
8. Top 3 motrices y top 3 dependientes
9. Ranking MDI → MII (gráfico de pendientes)
10. Mapa de desplazamientos entre los cuatro planos
11. Comparación con incidencia / favorabilidad (2 × 2)
12. Las seis variables críticas
13. El orden de la estrategia
14. Cierre

## Datos editables

Al inicio del `<script>`: `VARS` (las 20 variables), `CRUCES` (los cinco cruces de la
matriz), `MDI` (posición relativa de cada variable en el plano directo), `DESP`
(trayectoria por los cuatro planos), `BUMP` (rankings MDI → MII) y `ESTAB` (estabilidad
por iteración).

**Nota:** las coordenadas de `MDI` y `DESP` son posiciones *relativas* construidas a
partir de los rankings y cuadrantes descritos en el documento, no las coordenadas
exactas que exporta MICMAC. Si se quiere fidelidad total, reemplazarlas con los valores
de las figuras 1, 3, 5 y 6 del documento.

## Diseño

Misma identidad SUSI que la Entrega 1 (paleta del empaque, sello original, serif de alto
contraste + sans humanista) con una decoración distinta: riel rayado vertical en el borde
izquierdo, cuadrícula fina como textura (la matriz), portada y conclusión en rojo profundo
y cierre en negro. Animaciones con CSS y Web Animations API: onda de la matriz, vuelo de
los puntos al plano, trazado de líneas y recorrido de trayectorias. Respeta
`prefers-reduced-motion`.
