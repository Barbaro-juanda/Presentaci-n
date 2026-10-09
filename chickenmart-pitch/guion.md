# Guion completo · Chickenmart conectado

Pitch ejecutivo final · 16 diapositivas · 5 expositores · ~13:35 hablados (cronómetro a 15:00).
También están dentro de la presentación: tecla `N`.

## Reparto

| Expositor | Diapositivas | Tiempo aprox. |
|---|---|---|
| Santiago | 1, 2, 3 y mitad de la 16 | 2:50 |
| Juan David | 4, 5 y mitad de la 16 | 2:30 |
| Carolina | 6, 7 y 14 | 2:40 |
| Nataly | 8, 12, 13 y coordina la 11 | 2:20 + 1:00 de demo |
| Orozco | 9, 10 y 15 | 2:15 |

Etiquetas: **[HECHO]** del diagnóstico · **[PROPUESTA]** del equipo · **[PENDIENTE]** por completar · **✳ ficticio/supuesto**.

## 01 · Portada

**Expone:** Santiago · **Tiempo:** 30 s

**Contenido en pantalla**

- Logo de Chicken Mart (gallo integrado a la «C»).
- Lema: «Chickenmart conectado: del peso recibido a la disponibilidad de venta».
- Equipo y orden de exposición: Santiago, Juan David, Carolina, Nataly, Orozco.
- Leyenda: HECHO · PROPUESTA · PENDIENTE · ✳ FICTICIO/SUPUESTO.
- «Nada de lo propuesto está instalado hoy en Chickenmart».

**Visual y animación**

Registro oscuro con malla vino. Sello del gallo extruido en 3D (20 capas vino bajo una cara crema) que flota y recibe un lustre cada 6,5 s. El lema se arma letra por letra desde el eje X. Debajo, un «pulso»: un punto viaja de la caja KG a la caja ✓ y el riel se llena en bucle (del peso recibido a la disponibilidad).

**Notas del orador**

> Buenas tardes. Somos Santiago, Juan David, Carolina, Nataly y Orozco, y durante el semestre trabajamos con Chickenmart S.A.S., en el Alto de Las Palmas, en Envigado: vende derivados del pollo en su punto físico, por WhatsApp, por su sitio web y con domicilios en moto propia.
> Hoy no venimos a mostrar tecnología por mostrarla. Venimos a pedir una decisión de inversión, y nuestro lema la resume: Chickenmart conectado, del peso recibido a la disponibilidad de venta.
> Una aclaración antes de empezar, y miren la leyenda de abajo: en pantalla separamos lo que es un hecho del diagnóstico, lo que es propuesta nuestra y lo que todavía está pendiente. Nada de lo que proponemos está instalado hoy en Chickenmart, y cada número de ejemplo está marcado como ficticio.

## 02 · Problema y diagnóstico

**Expone:** Santiago · **Tiempo:** 55 s

**Contenido en pantalla**

- Titular: «No falta tecnología. Falta conexión.» [HECHO]
- Ya hay datos digitales de cada producto: SKU, peso, precio, proveedor, vencimiento.
- El inventario vive en archivos y se confirma contando.
- Al recibir mercancía, el inventario se actualiza después.
- Punto físico, WhatsApp, web y domicilios no están sincronizados.
- Las personas conectan todo a mano: con más productos y canales, no escala.

**Visual y animación**

Tres medidores semicirculares: el arco se llena y la aguja cae con rebote elástico (media · baja · baja). Debajo, cinco «islas» (recepción, inventario, disponibilidad, pedidos, ventas) unidas por cortes punteados con una mano que sube y baja: personas uniendo datos.

**Notas del orador**

> Empecemos por lo que encontramos. Chickenmart no está en cero: ya tiene sus productos en digital, con SKU, peso, presentación, precio, proveedor y vencimiento. Por eso su digitalización es media.
> El problema está en lo que pasa entre una cosa y otra. El inventario vive en archivos y se confirma contando. Los canales no están sincronizados. Y cuando llega mercancía, el inventario se actualiza después, no en el momento. Automatización baja, integración baja.
> Entonces el problema no es falta de tecnología: es fragmentación. No hay una única fuente que conecte recepción, inventario, disponibilidad, pedidos y ventas. Esas manitos de la imagen son personas uniendo la información a mano. Hoy funciona, pero cada producto, proveedor o canal nuevo le suma una costura más.

## 03 · AS IS → TO BE

**Expone:** Santiago · **Tiempo:** 55 s

**Contenido en pantalla**

- Titular: «De un proceso que se corta a uno que no se detiene.»
- AS IS [HECHO]: necesidad de compra → pedido al proveedor → recepción → inventario se actualiza después. Dolores: venta con verificación manual, sin reservas centralizadas, mínimos y vencimientos dependen de personas.
- TO BE [PROPUESTA]: recepción → pesaje neto confirmado → inventario central → disponibilidad vendible → reserva → salida real y conciliación.

**Visual y animación**

Dos flujos lado a lado. AS IS en cuadros grises con vía punteada; el paso 4 «después» tiembla y lleva un reloj que parpadea. TO BE en círculos vino: la vía se dibuja de arriba abajo y un pulso recorre los seis pasos en bucle.

**Notas del orador**

> Así se ve hoy el proceso, a la izquierda. Nace una necesidad de compra, se pide al proveedor, llega la mercancía… y el inventario se actualiza después. Mientras tanto, para vender, alguien verifica a mano si hay. No hay reservas centralizadas, así que dos canales pueden ofrecer lo mismo. Y estar pendiente de mínimos y vencimientos depende de la memoria de las personas.
> A la derecha está el proceso que proponemos, que es uno solo para todos los canales: se recibe, se pesa y se confirma el peso neto, eso entra a un inventario central, de ahí sale la disponibilidad vendible, el pedido reserva, y al despachar se registra la salida real y se concilia.
> Fíjense en la diferencia: a la izquierda la línea se corta; a la derecha el dato no se detiene.
> RELEVO → Juan David. Cierra así: «Ese es el qué. Juan David les muestra cómo se construye».

## 04 · Arquitectura e IoT

**Expone:** Juan David · **Tiempo:** 60 s

**Contenido en pantalla**

- Titular: «Una sola fuente de verdad para vender. Lo demás lee copias.» [PROPUESTA]
- Regla de oro: se vende solo desde el inventario central; Data Hub y Power BI nunca deciden un saldo.
- Báscula [PENDIENTE · por verificar]: celda de carga, no identifica el producto; la persona selecciona o escanea; tara y peso estable; salida USB · RS-232 · Bluetooth · red; sin conexión, cola local con ID único.
- «Tener wifi no garantiza integración».

**Visual y animación**

Diagrama de dos capas. Los cables se trazan solos y los paquetes de datos viajan por ellos (de ida y vuelta entre el inventario y los canales). El inventario central late con un aura. La copia hacia la capa analítica es una línea punteada que fluye.

**Notas del orador**

> Gracias, Santiago. La arquitectura tiene dos capas. Arriba, la operativa: la báscula, una interfaz de captura y el inventario central con el gestor de pedidos, que habla en los dos sentidos con la web, la caja y WhatsApp. Abajo, la analítica: los movimientos se copian a un Data Hub, que alimenta Power BI, la IA, los agentes y el gemelo digital.
> La regla de oro: se vende solo desde el inventario central. El Data Hub y Power BI leen copias; nunca deciden un saldo.
> Sobre la báscula, seamos precisos: pesa con una celda de carga, pero no sabe qué producto tiene encima. Una persona lo selecciona o lo escanea, se descuenta la tara y se espera peso estable. Cómo saca el dato, si por USB, RS-232, Bluetooth o red, está por verificar: tener wifi no garantiza integración. Y si se cae la conexión, el registro queda en cola local con un identificador único para que no se duplique.

## 05 · Automatizaciones A1–A3

**Expone:** Juan David · **Tiempo:** 60 s

**Contenido en pantalla**

- Titular: «Convertir el peso recibido en un registro fiable y una disponibilidad de venta actualizada.» [PROPUESTA · ejemplos ficticios]
- A1 Recepción: SKU › proveedor/lote/vto. › peso estable › tara › confirmación humana › 1 registro. 21,62 − 1,62 = 20,00 kg ✳ ficticio.
- A2 Reservas: vendible = físico − reservado − bloqueado − colchón*. 20 − 4 − 1 = 15 kg ✳ ficticio. Reserva al confirmar; salida con peso real; sin doble descuento; solo un canal gana.
- A3 Alertas por reglas: stock < X kg o lote a Y días → administradora. X e Y [PENDIENTE] los define el negocio.

**Visual y animación**

Tres tarjetas. A1: lector de báscula con «PESO ESTABLE» parpadeando y cifras que cuentan hasta 21,62 / 1,62 / 20,00 kg. A2: barra apilada que se reparte en vendible 15 · reservado 4 · bloqueado 1. A3: alarma con onda expansiva.

**Notas del orador**

> Sobre esa arquitectura corren tres automatizaciones. A1, la recepción: se elige el SKU, se registran proveedor, lote y vencimiento, se espera el peso estable, se descuenta la tara y una persona confirma. Sale un único registro. En el ejemplo, que es ficticio: veintiuno sesenta y dos en la báscula, menos uno sesenta y dos de la canastilla, quedan veinte kilos netos.
> A2, las reservas entre canales. Lo vendible es lo físico menos lo reservado, menos lo bloqueado y menos un colchón, si el negocio decide tenerlo. Con veinte kilos, cuatro reservados y uno bloqueado, se pueden vender quince. Se reserva al confirmar el pedido y se descuenta con el peso real cuando se entrega o sale en la moto, sin descontar dos veces. Si dos canales piden lo mismo al tiempo, solo uno gana.
> A3 son alertas por reglas: bajo un mínimo de X kilos o un lote a Y días de vencer, se avisa a la administradora. X e Y los define el negocio.
> RELEVO → Carolina. Cierra así: «Eso pasa dentro del local. Carolina les cuenta dónde viven esos datos».

## 06 · Estrategia cloud

**Expone:** Carolina · **Tiempo:** 45 s

**Contenido en pantalla**

- Titular: «Los datos, en un solo lugar. La decisión, siempre humana.» [PROPUESTA]
- Fuentes: punto físico, web, WhatsApp, pesaje, ajustes y mermas → base de datos central → automatizaciones con IA → dashboard y alertas → decisión humana.
- Beneficios: centralización, acceso, integración de canales, escalabilidad, respaldo.
- [PENDIENTE] Plataforma definitiva: se elige tras validar qué usa hoy Chickenmart.

**Visual y animación**

Tubería horizontal: cinco fuentes convergen en la base de datos central; los paquetes fluyen por cada etapa hasta la «decisión humana» en crema. Fila de cinco beneficios abajo.

**Notas del orador**

> Gracias, Juan David. La estrategia cloud se lee de izquierda a derecha. Entran cinco fuentes: el punto físico, la web, WhatsApp, el pesaje y los ajustes y mermas. Todo llega a una base de datos central. Encima corren las automatizaciones, algunas con IA. Eso termina en un tablero con alertas, y al final siempre decide una persona.
> ¿Qué gana Chickenmart? Centralización, porque hay un solo lugar donde mirar. Acceso desde cualquier punto. Integración de los canales. Escalabilidad, para crecer en productos sin rehacer el sistema. Y respaldo de la información.
> Algo importante: no estamos casando a Chickenmart con un proveedor. La plataforma definitiva se elige después de validar qué herramientas usa hoy la empresa, para aprovecharlas y no duplicarlas.

## 07 · Inteligencia artificial IA1–IA3

**Expone:** Carolina · **Tiempo:** 55 s

**Contenido en pantalla**

- Titular: «La IA estima y avisa. Una persona decide.» [PROPUESTA · gráficos ilustrativos]
- IA1 Pronóstico de demanda por producto: estimación con incertidumbre → alerta de reposición.
- IA2 Diferencias inusuales (peso recibido vs. ventas, ajustes, mermas, conteos): pide revisión, no acusa.
- IA3 Riesgo de no vender antes del vencimiento: prioriza lotes para rotación autorizada.
- Regla (A3) ≠ IA. Requiere histórico confiable. Nunca decide sola.

**Visual y animación**

Tres mini-gráficos ilustrativos (sin datos): IA1 la línea se dibuja y aparece la banda de incertidumbre; IA2 los puntos caen sobre la diagonal y uno fuera de rango se enciende con un anillo de alerta; IA3 barras de lotes que crecen hasta la línea de vencimiento. Franja «Regla ≠ IA».

**Notas del orador**

> Proponemos tres usos de inteligencia artificial, y los tres terminan en una persona. IA1 pronostica la demanda por producto. No da un número exacto: da una estimación con su margen de incertidumbre, que es esa banda, y con eso sugiere cuándo reponer.
> IA2 detecta diferencias inusuales entre lo que se recibió pesado, lo vendido, los ajustes, las mermas y los conteos. Cuando algo no cuadra, pide revisión; no acusa a nadie.
> IA3 estima el riesgo de que un lote no se venda antes de vencer, y prioriza esos lotes para una rotación que alguien autoriza.
> Abajo está la diferencia que nos importa que quede clara: una alerta por fecha o por mínimo es una regla, la A3 que vimos con Juan David. Estimar cuánto no se va a vender es IA. Y la IA necesita algo que hoy no existe: histórico confiable. Por eso va después del pesaje.
> RELEVO → Nataly. Cierra así: «La IA sugiere. Nataly les muestra quién actúa sobre esas sugerencias».

## 08 · Agentes G1–G3

**Expone:** Nataly · **Tiempo:** 45 s · **PENDIENTE**

**Contenido en pantalla**

- Titular: «Los agentes preparan. Las personas aprueban.» [PROPUESTA · PENDIENTE]
- Tabla objetivo · acción · quién aprueba: G1 Abastecimiento (propuesta de compra → gerencia aprueba); G2 Atención y pedidos (consulta stock, arma pedido, reserva, escala casos especiales → rol por definir); G3 Control operativo (sigue incidencias hasta cerrarlas → rol por definir).
- Recuadro: «Contenido pendiente de Nataly».

**Visual y animación**

Tabla de tres agentes con anillos orbitales que giran. Columna «quién aprueba» con check sólido (gerencia) o círculo punteado (por definir). Recuadro pendiente con cinta de obra animada.

**Notas del orador**

> [PENDIENTE · Nataly completa el contenido final de esta lámina.]
> Gracias, Carolina. Un agente es un asistente que, además de avisar, prepara una acción. Proponemos tres, y lo que más importa es la última columna: quién aprueba.
> G1, abastecimiento: con el stock y las alertas, prepara una propuesta de compra; la gerencia la aprueba o la ajusta.
> G2, atención y pedidos: consulta el stock disponible, arma el pedido y lo reserva; cuando el caso es especial, lo escala a una persona.
> G3, control operativo: sigue cada incidencia, como una diferencia de peso o una alerta, hasta que alguien la cierra.
> Ningún agente compra, cobra ni corrige inventario por su cuenta.

## 09 · Data Hub y Power BI

**Expone:** Orozco · **Tiempo:** 45 s · **PENDIENTE**

**Contenido en pantalla**

- Titular: «Cada movimiento deja rastro. El tablero lo vuelve visible.» [PROPUESTA · PENDIENTE]
- Modelo: productos, lotes, movimientos, pedidos.
- Tablero: existencias, disponibilidad, reservas, movimientos, merma por vencimiento, alertas, fecha de última actualización.
- ✳ Datos de prueba ficticios, del prototipo de Juan David.
- Recuadro: «Contenido pendiente de Orozco».

**Visual y animación**

Modelo entidad-relación de cuatro bloques (movimientos en vino) con relaciones que se trazan. Tablero de Power BI en esqueleto: seis tiles con brillo de «cargando» y la fecha de última actualización vacía.

**Notas del orador**

> [PENDIENTE · Orozco completa el contenido final de esta lámina.]
> Gracias, Nataly. Todo lo que hemos visto deja rastro, y aquí se ordena. El modelo de datos tiene cuatro piezas: productos, lotes, movimientos y pedidos. El movimiento es el corazón: cada entrada, reserva, salida, merma o corrección es una fila con su lote y su pedido.
> Sobre ese modelo va el tablero de Power BI: existencias, disponibilidad, reservas, movimientos, merma por vencimiento y alertas. Y arriba, siempre visible, la fecha de la última actualización, porque un tablero sin fecha invita a decidir con datos viejos.
> Los datos de prueba son ficticios y vienen del prototipo de Juan David. El tablero lee copias: nunca decide un saldo.

## 10 · Gemelo digital

**Expone:** Orozco · **Tiempo:** 45 s · **PENDIENTE**

**Contenido en pantalla**

- Titular: «Ensayar la decisión antes de tomarla.» [PROPUESTA · PENDIENTE]
- E1 Aumento de demanda · E2 Retraso de proveedor · E3 Compra adicional vs. vencimiento.
- Columnas: situación base → cambio → resultado → decisión (celdas «por simular»).
- Recuadro: «Contenido pendiente de Orozco».

**Visual y animación**

Matriz de 3 escenarios × 4 columnas que se arma por filas; las celdas «por simular» son esqueletos que cargan. Icono de gemelo (dos cuadros, uno sólido y otro punteado que se desplaza).

**Notas del orador**

> [PENDIENTE · Orozco completa los resultados de las simulaciones.]
> El gemelo digital es una copia del inventario donde se puede ensayar sin tocar el real. Preparamos tres escenarios, y los tres se leen igual: situación base, qué cambia, qué resulta y qué decisión sugiere.
> Uno: aumenta la demanda. Dos: el proveedor se retrasa. Tres: comprar más para aprovechar un precio, contra el riesgo de que se venza.
> Las celdas grises están pendientes porque los resultados todavía no están simulados, y no vamos a inventarlos. Lo que sí queda claro es para qué sirve: decidir antes de que pase, no después.
> RELEVO → Nataly. Cierra así: «Eso es lo que proponemos. Nataly les muestra lo que ya funciona».

## 11 · Implementación: demo integrada

**Expone:** Todos · coordina Nataly · **Tiempo:** 60 s

**Contenido en pantalla**

- Titular: «Un caso, de punta a punta. Lo probado y lo que falta.»
- Caso común (9 pasos): recepción pesada → comprobar saldo → reservar pedido → registrar salida → actualizar tablero → detectar riesgo → agente propone → persona valida → simular escenario.
- Prototipo de Juan David (Python + SQLite, ✳ datos ficticios), 12 pasos verificados: recepción de 20 kg, rechazo de duplicados, reservas con 15 kg vendibles, venta simultánea con un solo ganador, despachos con peso real, cancelación, merma, corrección autorizada, alertas. No instalado en Chickenmart.
- [PENDIENTE] Evidencias de IA (Carolina), agentes (Nataly), tablero y gemelo (Orozco).

**Visual y animación**

Riel de nueve pasos que se llena de izquierda a derecha mientras los círculos aparecen; el paso 8 (persona valida) va relleno. Lista de checks del prototipo que se marcan uno a uno.

**Notas del orador**

> Gracias, Orozco. Ahora, un caso de punta a punta, el mismo para todos. Arriba están los nueve pasos: registrar una recepción pesada, comprobar el saldo, reservar un pedido, registrar la salida, actualizar el tablero, detectar un riesgo, que el agente proponga una acción, que una persona la valide y simular un escenario.
> ¿Qué está probado hoy? El prototipo de Juan David, en Python con SQLite y con datos ficticios, verificó doce pasos: entre ellos la recepción de veinte kilos, el rechazo de duplicados, quince kilos vendibles con reservas, una venta simultánea con un solo ganador, despachos con peso real, una cancelación, una merma, una corrección autorizada y las alertas.
> [Turno de cada uno, 10 segundos: Juan David muestra la recepción; Carolina, Nataly y Orozco, su parte cuando la tengan.]
> Las demás evidencias están pendientes, y lo decimos así. Y recuerden: es un prototipo del equipo, no está instalado en Chickenmart.

## 12 · Roadmap

**Expone:** Nataly · **Tiempo:** 45 s · **PENDIENTE**

**Contenido en pantalla**

- Titular: «Primero la base. Después la inteligencia.» [FASES SUGERIDAS · PENDIENTE]
- 1 Validar proceso, catálogo y datos · 2 Piloto de pesaje e inventario central · 3 Integrar canales y tablero · 4 IA, agentes y gemelo · 5 Medir y ajustar.
- Piloto (fases 1–2): 8–12 semanas ✳ supuesto, no compromiso.
- Recuadro: «Contenido pendiente de Nataly».

**Visual y animación**

Cinco chevrones que entran en secuencia; la fase 2 (piloto) en vino. Barra de Gantt: piloto sólido con «8–12 semanas ✳ supuesto», resto punteado «por definir».

**Notas del orador**

> [PENDIENTE · Nataly completa el roadmap final.]
> El roadmap tiene cinco fases y el orden no es casual. Primero se valida: el proceso real, el catálogo y la calidad de los datos. Segundo, el piloto de pesaje e inventario central, que es lo que pedimos aprobar. Tercero, se integran los canales y el tablero. Cuarto, entran la IA, los agentes y el gemelo, que solo sirven cuando ya hay histórico confiable. Y quinto, se mide y se ajusta.
> Como referencia, un piloto así podría tomar de ocho a doce semanas. Es un supuesto, no un compromiso: el tiempo real sale de la fase uno.

## 13 · Riesgos y controles

**Expone:** Nataly · **Tiempo:** 50 s · **PENDIENTE**

**Contenido en pantalla**

- Titular: «Cada riesgo, con su control.» [CONTROLES · PENDIENTE matriz final]
- Riesgos R1–R9: báscula sin salida de datos, tara o referencia incorrecta, registros duplicados, ventas no registradas, desconexión, datos antiguos, IA errónea o falsas alertas, accesos indebidos, poca información histórica.
- Controles: ID único, confirmación humana, cola offline, permisos por rol, revisión humana.
- Escala: probabilidad e impacto de 1 a 3; celda = P × I (1–2 bajo, 3–4 medio, 6–9 alto). Ubicación pendiente de Nataly.

**Visual y animación**

Matriz 3×3 de probabilidad × impacto que se calienta en diagonal (hueso → crema → vino) con el sello «Ubicación pendiente» que cae encima. Las fichas R1–R9 caen con rebote en una bandeja «sin ubicar». Cinco controles en bloques vino.

**Notas del orador**

> [PENDIENTE · Nataly ubica cada riesgo en la matriz final.]
> Ya identificamos nueve riesgos. Algunos son técnicos: que la báscula no tenga salida de datos, una tara o una referencia mal elegida, registros duplicados o una desconexión. Otros son de operación: ventas que no se registran o datos viejos. Y otros, de la parte inteligente: que la IA se equivoque o dé falsas alertas, accesos indebidos y poca información histórica.
> La matriz cruza probabilidad e impacto, de uno a tres cada uno, y el color sube con el producto de ambos. La ubicación final de cada riesgo está pendiente.
> Lo que sí está definido son los controles: un ID único por registro, confirmación humana, cola sin conexión, permisos por rol y revisión humana de lo que sugiera la IA.
> RELEVO → Carolina. Cierra así: «Con los riesgos sobre la mesa, Carolina les muestra cuánto cuesta y cómo lo medimos».

## 14 · Costos, KPIs y ROI

**Expone:** Carolina · **Tiempo:** 60 s

**Contenido en pantalla**

- Titular: «Sin precios inventados. Con la fórmula lista para los reales.» [ESTRUCTURA · PENDIENTE valores]
- Costos: inversión inicial (báscula, instalación, integración de inventario y canales, base de datos, migración, automatizaciones, capacitación), recurrentes (nube, licencias, IA, mantenimiento, soporte) y contingencia. Costo año 1 = inicial + recurrentes + contingencia = $ — (por cotizar).
- KPIs: diferencia físico vs. registro (kg), tiempo de recepción, pedidos afectados por agotados, merma por vencimiento (kg), demora de actualización, error de pronóstico. Metas después de medir la línea base.
- ROI = (beneficio neto / inversión) × 100 · Payback = inversión / ahorro mensual neto. Calculables solo con datos reales.

**Visual y animación**

Tres columnas: chips de costos con la ecuación en una caja negra con espacios «$ —» que parpadean; seis KPIs con «base: por medir»; dos fórmulas (ROI y payback) escritas como fracciones.

**Notas del orador**

> Gracias, Nataly. Vamos con plata, y con honestidad: no tenemos precios confirmados, así que no vamos a poner cifras que no existen. Lo que traemos es la estructura para calcularlo bien.
> Los costos son de tres tipos. La inversión inicial: báscula, instalación, integración de inventario y canales, base de datos, migración, automatizaciones y capacitación. Los recurrentes: nube, licencias, IA, mantenimiento y soporte. Y una contingencia. El costo del primer año es la suma de los tres.
> Para saber si funcionó, seis indicadores: diferencia entre lo físico y lo registrado en kilos, tiempo de recepción, pedidos afectados por agotados, kilos de merma por vencimiento, demora en actualizar y error de pronóstico. Las metas se fijan después de medir la línea base.
> Y el retorno se calcula con estas dos fórmulas: ROI y periodo de recuperación. Las dos se pueden resolver solo con datos reales, y eso es justamente lo que deja la fase uno.
> RELEVO → Orozco. Cierra así: «Eso es lo que cuesta. Orozco les muestra hacia dónde lleva».

## 15 · Industria 5.0 y visión a 5 años

**Expone:** Orozco · **Tiempo:** 45 s · **PENDIENTE**

**Contenido en pantalla**

- Titular: «Tecnología al servicio de quien trabaja.» [PROPUESTA · PENDIENTE]
- Personas: el trabajador verifica y aprueba · Sostenibilidad: medir y reducir desperdicio · Resiliencia: operar ante cortes.
- Visión a 5 años: inventario común → canales coordinados → trazabilidad por lote → compras con datos → crecimiento con control. Sin prometer nuevas sedes.
- Recuadro: «Contenido pendiente de Orozco».

**Visual y animación**

Tres pilares con icono lineal (persona, hoja, escudo). Ruta de cinco hitos que se encienden en secuencia hasta «crecimiento con control».

**Notas del orador**

> [PENDIENTE · Orozco completa el contenido final de esta lámina.]
> Gracias, Carolina. La Industria 5.0 pone a la persona en el centro, y en Chickenmart eso se traduce en tres cosas. Personas: el trabajador verifica y aprueba; la tecnología le quita la tarea repetitiva, no la decisión. Sostenibilidad: medir el desperdicio por vencimiento para poder reducirlo. Y resiliencia: seguir operando aunque se caiga la conexión.
> Hacia cinco años, la visión es: un inventario común, canales coordinados, trazabilidad por lote, compras con datos y crecimiento con control. No prometemos nuevas sedes: prometemos que, si Chickenmart decide crecer, lo haga sobre una base que aguanta.
> RELEVO → Santiago. Cierra así: «Esa es la visión. Santiago y Juan David les dicen qué necesitamos hoy».

## 16 · Decisión de inversión

**Expone:** Santiago y Juan David · **Tiempo:** 60 s

**Contenido en pantalla**

- Titular: «Aprobar un piloto por fases que empiece por pesaje conectado e inventario central.» [RECOMENDACIÓN]
- Problema: información fragmentada, conectada a mano.
- Evidencia: prototipo con 12 pasos verificados sobre datos ficticios.
- Viabilidad: por fases, con confirmación humana y controles; costos por cotizar.
- Resultado esperado: disponibilidad de venta confiable, medida contra una línea base.
- Cierre con el lema.

**Visual y animación**

Registro vino. Cuatro bloques (problema, evidencia, viabilidad, resultado). La pila se construye desde la base: primero «pesaje conectado + inventario central» en crema y luego caen encima IA, agentes, tablero y gemelo. Cierre con el sello pequeño y el lema.

**Notas del orador**

> SANTIAGO: Llegamos a lo que venimos a pedir. Nuestra recomendación es aprobar un piloto por fases que empiece por el pesaje conectado y el inventario central. ¿Por qué ahí? Porque es la base: la IA, los agentes, el tablero y el gemelo dependen de que el dato de inventario sea confiable. Sin esa base, todo lo demás se construye sobre arena.
> JUAN DAVID: En cuatro bloques. El problema: la información está fragmentada y la conectan personas a mano. La evidencia: un prototipo con doce pasos verificados, con datos ficticios. La viabilidad: por fases, con confirmación humana, controles definidos y costos que se cotizan antes de comprometer más. Y el resultado esperado: una disponibilidad de venta confiable en todos los canales, medida contra una línea base.
> SANTIAGO: Chickenmart conectado: del peso recibido a la disponibilidad de venta. Muchas gracias. [Pausa de dos segundos y abrir preguntas.]
