# Prompt para consultar con Claude

Copia todo lo que está entre las líneas y pégalo en una conversación nueva.

---

Necesito que me asesores como director de arte. No quiero que escribas código:
quiero que conversemos hasta tener una dirección visual clara que yo después le
pueda pasar a otra persona para que la construya.

## El contexto

Soy estudiante de Digital Business & Administration en ESIC. Para la materia de
Prospectiva 1 analizamos a **SUSI Panadería Artesanal**, una empresa real de
Medellín, y ahora quiero presentarle los resultados **a la CEO de la empresa,
Susanne Seifert**. Son 10 minutos, 12 diapositivas, y exponemos tres personas.

No es una sustentación académica. Es una reunión de negocio donde le vamos a
pedir luz verde para tres decisiones concretas.

## Qué es SUSI

- Panadería y repostería artesanal fundada en **1985** en Medellín por Susanne
  Seifert, colombiana de ascendencia alemana con formación técnica en panadería
  en Europa y Estados Unidos.
- Recetas europeas: pan de doble centeno, brezel, torta Selva Negra.
- Planta propia en Itagüí. Seis líneas: panadería, crocantes, tortas, cereales
  de desayuno (Happy Mix), snacks de cereales soplados y congelados.
- Sin conservantes, colorantes artificiales ni grasas trans.
- Vende por dos canales: uno propio (tienda en línea, domicilios y WhatsApp,
  limitado al Valle de Aburrá) y uno moderno (doce cadenas: Éxito, Carulla,
  Euro, Olímpica, Colsubsidio, Farmatodo).
- Su empaque más reconocible es una bolsa naranja con una banda azul que dice
  «70 % menos azúcar». También tiene una línea de cereal en bolsa de papel kraft
  con etiqueta negra, y el logotipo de la marca es una **serif**.

## Qué dice la presentación

Es una sola historia que avanza así:

1. Portada
2. **La tesis:** 12 de los 15 puntos de contacto con el consumidor son de
   terceros. Solo 3 son de SUSI.
3. Lo que es SUSI hoy (1985, 12 cadenas, 6 líneas, 0 sellos de advertencia)
4. Por qué no puede competir por precio: cuesta 3,58× el pan empacado masivo
5. De dónde viene el costo: Colombia importa ~99 % del trigo que consume
6. El método: 20 variables, 400 cruces, 6 palancas
7. El hallazgo: controla sus palancas, no controla su margen
8. Tres futuros al 2030
9. El escenario más probable y más peligroso: «erosión lenta»
10. Hoja de ruta: 8 decisiones, 7 en 18 meses
11. Lo que pedimos: 3 movimientos este trimestre
12. Cierre

## Lo que ya tengo y qué pasó

Ya hay una versión construida. La hicimos así y **no me convenció**:

- **Paleta:** saqué los colores de fotos de los empaques reales (naranja
  `#E43018`, azul `#0078CC`, ámbar `#E4A80C`, kraft, rojo de marca `#D83624`).
  Esa parte me parece bien.
- **Cinco fondos distintos** repartidos entre las 12 láminas: papel kraft,
  casi blanco, negro, azul profundo y rojo. La idea era que cada fondo
  correspondiera a una función del relato.
- **Tipografía:** Fraunces (serif) para titulares y cifras, Inter para cuerpo,
  JetBrains Mono para datos.
- **Animación:** los titulares y las cifras se arman letra por letra, entrando
  desde el espacio 3D con desenfoque, como un reveal de logo de After Effects.
- Metí **fotos de producto recortadas de un catálogo** y quedaron mal: mal
  recortadas y fuera de lugar. Ya las quité.
- También hice unos **gráficos**: un anillo con 15 puntos donde 12 se
  desprenden hacia afuera (para la tesis), barras de precio, un diagrama de
  Gantt para la hoja de ruta. **No me terminaron de gustar** y no sé bien si el
  problema es la idea, la ejecución, o que sobran.

## Lo que quiero resolver contigo

Ayúdame a decidir, con criterio y explicándome el porqué:

1. **¿Imágenes sí o no?** Si sí, ¿qué tipo exactamente — fotografía de producto,
   de proceso, de la planta, retrato, textura, nada de eso? ¿Y cuántas, y en qué
   láminas? Si no, ¿con qué se sostiene visualmente una presentación de 12
   láminas sin fotos y sin que se vea como un documento de Word?
2. **¿Cómo represento la tesis de 12/15 puntos de contacto?** Es el dato más
   importante del deck. El anillo con puntos no me convenció. ¿Qué otra forma
   hay de que ese número se sienta?
3. **¿Cinco fondos distintos es buena idea o es un desorden?** ¿Cuántos
   registros de color debería tener realmente un deck de 12 láminas?
4. **¿La animación letra por letra le sirve a una reunión con una CEO, o es
   ruido?** ¿Qué nivel de movimiento es el correcto acá?
5. **¿Qué haría que esto se vea como SUSI y no como cualquier presentación de
   consultoría?** La marca es artesanal, con 40 años y origen alemán. No quiero
   que se vea ni genérica ni como una startup.

## Cómo quiero que trabajemos

- Hazme preguntas antes de proponer. Si algo no te cuadra, dímelo.
- Cuando propongas, dame **dos o tres direcciones distintas**, no una sola, y
  explícame qué gana y qué pierde cada una.
- Sé concreto: colores en hex, nombres de tipografías, descripciones de
  composición. Nada de «usa un diseño limpio y moderno».
- No escribas código. Al final quiero un **resumen de la dirección acordada**
  que yo pueda copiar y pasarle a quien lo va a construir.

## Restricciones técnicas de quien lo construye

Para que no propongas algo imposible:

- Es un archivo HTML único y autónomo. Sin servidor, sin conexión, sin CDN.
- Lienzo fijo de 1920×1080, escalado a la pantalla.
- Solo se pueden animar `opacity`, `transform`, `clip-path` y filtros. Hay GSAP.
- Las tipografías tienen que poder descargarse como `.woff2` e incrustarse.
  Ahora mismo hay disponibles: Fraunces, Inter, Space Grotesk, JetBrains Mono,
  Nunito y Kalam. Se pueden conseguir otras de Google Fonts.
- Si propones imágenes, yo tengo que conseguirlas: dime exactamente cuáles pedir
  o fotografiar.

---
