# Análisis del entorno, incidencia y favorabilidad — SUSI S.A.S.

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
(`index.html` en la raíz solo redirige a ese archivo, para que funcione el despliegue en Vercel / GitHub Pages.)

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
