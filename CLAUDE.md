# Estudio de presentaciones · Juan David Escobar

Este repositorio es donde viven **todas** las presentaciones de Juan David (ESIC, Digital Business).
Se publica solo en Vercel desde `main`: https://presentaci-n-five.vercel.app

- `index.html` (raíz): el inicio, una biblioteca con todas las presentaciones.
- `guia/index.html`: la guía visual de cómo se hacen. Este archivo es su versión corta para trabajar.
- Cada presentación vive en su carpeta: `marca-tema/index.html` (las tres primeras, de SUSI y Juan Valdez, son archivos sueltos en la raíz).

Juan David escribe en español y todo se entrega en español.

## Principios

1. **Una historia que pide algo.** Problema → evidencia → propuesta → decisión. El cierre dice qué se aprueba o qué nos llevamos.
2. **Una idea por diapositiva.** El titular es una afirmación. Máximo 5 bullets cortos y un solo visual por diapositiva.
3. **Nada inventado.**
   - Cada dato lleva su fuente (página, documento o minuto de la entrevista, en el pie o en mono pequeño).
   - Los números de ejemplo van marcados `✳ ficticio` / `✳ supuesto` / `preliminar`.
   - Una cita no textual dice «paráfrasis».
   - Si falta contenido, se pone un recuadro «Contenido pendiente de [nombre]» y se pregunta; nunca se rellena.
4. **La marca del cliente manda.** La paleta, la tipografía y los motivos salen del logo, el empaque o la tienda real. Nada de plantillas genéricas.
5. **Motion graphics con sentido.** Un clic = una escena completa, sin sub-pasos, con una coreografía GSAP de menos de 10 s y un bucle ambiental suave.
6. **Se expone, no se lee.** Cada diapositiva lleva su guion dentro (`N`), con tiempo, expositor y `RELEVO →`.
7. **Cada detalle importa.**
   - Al editar se mantiene exactamente el mismo diseño, colores y tipografía.
   - No se toca una diapositiva que no se pidió cambiar.
   - Si se ve una incoherencia en otra diapositiva, se avisa en vez de arreglarla por cuenta propia.

## Técnica

- **Lienzo y archivos:** fijo de 1920 × 1080, escalado a la ventana. HTML autónomo; fuentes `.woff2` y GSAP 3.12.5 locales, sin CDN. Las fuentes compartidas están en `fonts/` y `chickenmart-pitch/vendor/gsap.min.js`.
- **Portal (el mismo en todas):**
  - Barra superior con cronómetro, Cuadrícula (`O`), Notas (`N`), Atajos (`?`) y Presentar (`P`).
  - Panel de miniaturas a la izquierda.
  - Teclas: `T`/`R` cronómetro, `F` pantalla completa, `Esc`. Enlace directo `index.html#N`.
- **Animación:**
  - Solo se animan `transform`, `opacity`, `clip-path` y filtros.
  - Respeta `prefers-reduced-motion`.
  - Safari entra en modo plano (sin 3D ni desenfoques); se fuerza con `?plano`.
- **Color:**
  - Máximo tres registros de fondo: claro para lo denso, oscuro para impacto, y un acento reservado para la decisión.
  - Todo texto con contraste ≥ 4,5:1. Se derivan tonos oscuros del color de marca para el texto pequeño.
- **Tipografía por defecto:** Nunito 900 (titulares y cifras), Inter (cuerpo, 24–30 px) y Space Mono (HUD, kickers, fuentes). Se usa una serif si la marca es artesanal o clásica.
- **Etiquetas, con forma y color:**
  - `HECHO`: cuadrado lleno.
  - `PROPUESTA`: círculo de acento.
  - `PENDIENTE`: triángulo, borde punteado y rayado.
  - `VALIDACIÓN REAL`: sello doble.
  - `✳ FICTICIO`.
- **Videos:** MP4 + WebM, `muted playsinline`. Arrancan al entrar y se pausan al salir; el clic sobre el video no avanza la diapositiva.
- **Imágenes:** solo si son buenas, recortadas y fundidas con el fondo. Nada de recortes de catálogo mal hechos.

## Flujo

1. **Brief:** materia, rúbrica, tiempo, personas, marca y fuente. Pregunta solo lo que cambia el resultado.
2. **Estructura:** diapositiva por diapositiva, con título, contenido, visual y notas. Se condensa para caber en el tiempo.
3. **Construcción:** en `marca-tema/`.
4. **Verificación:**
   - Capturas con Playwright (`require('/opt/node22/lib/node_modules/playwright')`; Chromium ya instalado, no correr `playwright install`).
   - Que nada se salga ni se corte, y consola sin errores.
5. **Publicación:**
   - Rama → PR → merge a `main`.
   - Portada en `inicio/portadas/<id>.jpg`: captura de la diapositiva 1 a 1280×720, con `P` pulsado para ocultar el portal.
   - Una entrada en la lista `DECKS` de `index.html`.
6. **Entregables extra:** PDF si lo piden (capturas 3840×2160 de cada diapositiva unidas en un PDF), guion en Google Docs para el equipo.

Al terminar, resumir los cambios por diapositiva (título, contenido, visual, notas) solo para lo nuevo o modificado.
