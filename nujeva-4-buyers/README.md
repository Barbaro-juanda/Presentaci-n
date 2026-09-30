# NUJEVA · Buyer Persona, mercado y arquitectura de consumidores

Presentación de **12 escenas por pasos** para exponer ante un jurado en
computador o proyector. Tiempo oral objetivo: 10 minutos.

Toda la información proviene del *Informe Buyer Persona Nujeva* (21 páginas,
versión con la sección 17, «Arquitectura ampliada de buyers»). No hay cifras,
competidores, certificaciones ni registros añadidos.

## Cómo abrirla

Doble clic en `index.html`. No necesita servidor, internet ni instalación:
GSAP, ScrollTrigger y las tres tipografías viajan dentro del archivo.

## Navegación · por pasos, no por scroll

Cada escena tiene entre 1 y 4 pasos. Avanzar revela el siguiente paso y, cuando
se acaban, pasa a la escena siguiente. La rueda del ratón también avanza de a un
paso, sin saltárselos.

| Tecla | Acción |
|---|---|
| `→` `↓` `espacio` · clic | Siguiente paso |
| `←` `↑` | Paso anterior |
| `Inicio` · `Fin` | Primer · último paso |
| `F` | Pantalla completa |
| `T` | Cronómetro 00:00 → 10:00 (oculto por defecto; se pone cálido en el último minuto) |
| `N` | Notas del orador |
| `R` | Reinicia el cronómetro |
| `Esc` | Cierra paneles |

El indicador de arriba a la derecha muestra la escena, no el paso: `05 / 12`.

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
├── fonts/              Fraunces · Inter · JetBrains Mono (licencia abierta)
├── vendor/             GSAP 3.12.5 y ScrollTrigger, en local
└── README.md
```

El proyecto no tiene toolchain de npm, así que las dependencias se vendorizaron
como archivos locales: el efecto es el mismo que `npm install` para el requisito
de no depender de un CDN durante la exposición.

## Encapsulado

Todo el CSS vive bajo `#nb` con prefijo `.nb-`, y las tipografías se registran
como `NB Serif`, `NB Sans` y `NB Mono`. Nada de esta carpeta afecta a las otras
presentaciones del repositorio.

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
