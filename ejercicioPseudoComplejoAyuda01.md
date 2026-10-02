**Ejercicio guiado de pseudocódigo — Caja de una tienda**

Diseña un algoritmo que gestione el cobro de una compra formada por varios productos. Para cada producto se introducirá su precio unitario y la cantidad de unidades. La compra terminará al introducir un precio de **0**.

**Requisitos**

- Si el precio es negativo, muestra un aviso y vuelve a pedirlo.
- Si el precio es 0, termina la introducción de productos sin solicitar unidades.
- Para cada precio positivo, solicita una cantidad entera de unidades mayor que 0. Si no es válida, vuelve a pedirla.
- Calcula el número total de unidades y el importe acumulado.
- Aplica un descuento según el importe de la compra:
  - Menos de 50 euros: sin descuento.
  - Desde 50 hasta menos de 100 euros: **5 %**.
  - Desde 100 euros: **10 %**.
- Muestra un resumen con las unidades, el importe antes del descuento, el porcentaje aplicado, el descuento en euros y el importe final.
- Si no se registra ningún producto, muestra «No se han registrado productos» en lugar del resumen.
- Utiliza las primitivas estudiadas. No necesitas validar entradas de texto ni redondear.

**Ejemplo de interacción**

```text
CAJA DE LA TIENDA

Introduce el precio unitario en euros (0 para terminar):
20
Introduce el número de unidades:
2
Introduce el precio unitario en euros (0 para terminar):
-5
El precio no puede ser negativo.
Introduce el precio unitario en euros (0 para terminar):
10
Introduce el número de unidades:
0
La cantidad debe ser mayor que 0.
Introduce el número de unidades:
3
Introduce el precio unitario en euros (0 para terminar):
0

RESUMEN DE LA COMPRA
Unidades compradas: 5
Importe antes del descuento: 70 euros
Descuento aplicado: 5 %
Descuento: 3.5 euros
Importe final: 66.5 euros
```

**Pistas para avanzar**

Lee una pista, intenta resolver esa parte y consulta la siguiente solo cuando la necesites.

**1. Identifica qué necesitas recordar**

Imagina que haces la compra con papel y lápiz. ¿Qué datos anotarías de cada producto? ¿Qué dos totales tendrías que conservar mientras introduces los siguientes?

Piensa también cuánto deben valer esos totales cuando todavía no has comprado nada.

**2. Distingue los tres significados del precio**

Un precio negativo, uno igual a cero y uno positivo no significan lo mismo.

Escribe con tus palabras qué debe ocurrir en cada caso. ¿En cuáles de ellos tiene sentido preguntar por las unidades?

**3. Separa las repeticiones**

Hay acciones que se repiten porque quedan productos y otras que se repiten porque un dato es incorrecto.

Para cada repetición, responde:

- ¿Qué obliga a seguir repitiendo?
- ¿Qué permite dejar de repetir?
- ¿Qué dato debe volver a solicitarse para que la situación pueda cambiar?

**4. Actualiza los totales en el momento adecuado**

Si compras tres unidades de un producto de 10 euros, ¿cuánto aumenta el importe? ¿Y el total de unidades?

Localiza el punto en el que ya sabes que tanto el precio como la cantidad son válidos. ¿Deberías actualizar los totales antes de llegar a él?

**5. Decide cuándo aplicar el descuento**

Si llevas gastados 40 euros, pero todavía puedes añadir productos, ¿conoces ya el descuento definitivo?

Antes de escribir las condiciones, clasifica a mano estas cantidades: **49, 50, 99 y 100 euros**. Cada una debe pertenecer a un único tramo.

**6. Prepara el cierre**

¿Cómo puedes saber si se ha comprado algo? ¿Qué mensaje corresponde si no hay productos?

Cuando sí hay compra, distingue tres conceptos: porcentaje de descuento, cantidad descontada e importe final.

**Comprueba tu propuesta**

Recorre tu algoritmo línea a línea con estos casos:

- Introducir 0 como primer precio.
- Introducir un precio negativo y después uno válido.
- Introducir varias cantidades incorrectas antes de una válida.
- Realizar una compra de exactamente 50 euros.
- Realizar una compra de exactamente 100 euros.

Anota cómo cambian las variables. Comprueba que ningún dato incorrecto modifica los totales y que nunca se piden unidades después de introducir un precio de 0.
