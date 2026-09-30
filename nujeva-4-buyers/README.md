# NUJEVA · Buyer Persona, mercado y arquitectura de consumidores

Presentación de **12 escenas por pasos** para exponer ante un jurado en
computador o proyector. Tiempo oral objetivo: 10 minutos.

Toda la información proviene del *Informe Buyer Persona Nujeva* (21 páginas,
versión con la sección 17, «Arquitectura ampliada de buyers»). No hay cifras,
competidores, certificaciones ni registros añadidos.

## Cómo abrirla

Doble clic en `index.html`. No necesita servidor, internet ni instalación:
GSAP, ScrollTrigger y las tres tipografías viajan dentro del archivo.

## Navegación · el mismo portal que las demás presentaciones

Barra superior con el cronómetro y los botones, panel lateral con las doce
diapositivas en miniatura, y el lienzo de 1920×1080 escalado al centro. El botón
**Presentar** oculta todo el chrome y entra en pantalla completa.

Dentro de cada escena el contenido entra **por pasos** (de 1 a 4). Avanzar revela
el siguiente y, al agotarlos, pasa a la escena siguiente. La rueda del ratón
avanza de a un paso, sin saltárselos.

| Tecla | Acción |
|---|---|
| `→` `↓` `espacio` · clic | Siguiente paso |
| `←` `↑` | Paso anterior |
| `Inicio` · `Fin` | Primer · último paso |
| `P` | Modo presentación |
| `O` | Vista de cuadrícula con las 12 escenas |
| `N` | Notas del orador |
| `T` | Cronómetro 00:00 → 10:00 (cálido en el último minuto, rojo al pasarse) |
| `F` | Pantalla completa |
| `R` | Reinicia el cronómetro |
| `Esc` | Cierra lo que esté abierto |

El indicador muestra la escena, no el paso: `05 / 12`.

## Las doce escenas

1. Portada · 2. El punto de partida · 3. Contexto de mercado ·
4. El error del buyer original · 5. Ecosistema de decisión · 6. Mateo y Marta ·
7. Miguel · 8. Andrés · 9. Mateo vs. Andrés · 10. Los cuatro buyers ·
11. Universo de marca y conclusión · 12. Próximos pasos *(saltable)*

El guion completo está en `speaker-notes.md`; sus dos frases guía por escena
alimentan el panel `N`.

## Etiquetas epistemológicas

Distinguibles por **color y forma**, no solo por color:

| Etiqueta | Forma | Significa |
|---|---|---|
| DATO | cuadrado | Cifra de fuente secundaria, con su referencia `[n]` |
| HALLAZGO | círculo | Lectura que el informe da por establecida |
| INTERPRETACIÓN | rombo | Lectura estratégica del equipo |
| HIPÓTESIS | triángulo + borde punteado | **No validado** |
| OPORTUNIDAD | chevron | Implicación accionable |

La asignación buyer → territorio y la ruta «de cuidador a consumidor» aparecen
siempre marcadas como hipótesis.

## Estructura

```
nujeva-4-buyers/
├── index.html          la presentación, autocontenida
├── speaker-notes.md    guion de ~10 minutos
├── fonts/              Space Grotesk · Fraunces · JetBrains Mono (licencia abierta)
├── vendor/             GSAP 3.12.5 y ScrollTrigger, en local
└── README.md
```

El proyecto no tiene toolchain de npm, así que las dependencias se vendorizaron
como archivos locales: el efecto es el mismo que `npm install` para el requisito
de no depender de un CDN durante la exposición.

## Dirección visual

«Noche cálida»: base azul-verde profunda (no negra), superficies de vidrio con
profundidad, un hilo de luz que recorre la aurora de verde a arcilla, y tipografía
**Space Grotesk** para la voz analítica con **Fraunces en cursiva** reservada
únicamente para la voz humana de los buyers. La intención es que se sienta
contemporáneo sin caer en estética hospitalaria, de farmacia ni de neón frío: la
calidez y la dignidad siguen siendo el centro.

## Encapsulado

Todo el CSS usa el scope `#nb` y el prefijo `.nb-`; las tipografías se registran
como `NB Display`, `NB Serif` y `NB Mono`. Los tokens de color viven en `:root`
porque el lienzo envuelve al contenedor `#nb`, pero el archivo es autónomo y no
comparte hoja de estilos con nada más del repositorio.

## Accesibilidad y robustez

- `prefers-reduced-motion`: todo visible, sin animación.
- Si el JavaScript falla, `#nb` conserva `.nb-plano` y el contenido se lee.
- Ninguna escena tiene scroll interno. Probada sin desbordes en 1920×1080 y
  1366×768.

## Reglas de contenido respetadas

No se afirma ni se insinúa que el producto prevenga sarcopenia, cure
enfermedades, recupere masa muscular, aumente la esperanza de vida o mejore
fuerza y energía. «Fuerza», «músculo» y «envejecimiento saludable» aparecen solo
como motivación del buyer. El informe advierte expresamente que no conviene
construir la propuesta sobre la frase «la sarcopenia empieza a los 40»: esa
frase no aparece en la presentación.
