**Pseudocódigo guiado paso a paso — Caja de una tienda**

Vas a crear un algoritmo para calcular el importe de una compra. Trabaja por pasos: escribe una parte, comprueba que la entiendes y continúa con la siguiente.

Para cada producto, pedirás su precio y sus unidades. Un precio de **0** indicará que la compra ha terminado.

**Paso 1. Prepara el algoritmo y las variables**

Escribe el inicio del algoritmo y un mensaje de bienvenida.

Necesitarás variables para guardar:

- El precio del producto que se está introduciendo.
- Las unidades de ese producto.
- El total de unidades de la compra.
- El importe acumulado de la compra.

Elige nombres descriptivos. Inicializa los dos totales pensando en esta pregunta: **si todavía no hay productos, cuántas unidades llevas y cuánto has gastado?**

**Paso 2. Solicita el primer precio**

Escribe un mensaje que indique que se debe introducir el precio y que **0 significa terminar**. Después, lee el dato.

No pidas todavía las unidades: primero debes comprobar el precio.

**Paso 3. Repite la petición si el precio es negativo**

Añade un bucle `Mientras` que se repita cuando el precio sea negativo.

Dentro de ese bucle:

1. Muestra un aviso.
2. Vuelve a mostrar la petición del precio.
3. Lee el nuevo precio.

Comprueba mentalmente qué sucede si el usuario introduce **−5, −2 y 10**, en ese orden. ¿Se conserva finalmente el 10? ¿Puede continuar también si introduce 0?

**Paso 4. Crea el bucle de la compra**

Una vez validado el precio, añade otro `Mientras` para procesar productos hasta que se introduzca 0.

Los pasos **5, 6 y 7** deben quedar dentro de este bucle. Utiliza la sangría para mostrarlo.

Piensa qué condición expresa: **«todavía no se ha introducido la señal de terminar»**.

**Paso 5. Solicita y comprueba las unidades**

Dentro del bucle de la compra:

1. Muestra un mensaje solicitando las unidades.
2. Lee la cantidad.
3. Añade un `Mientras` para repetir la petición si la cantidad no es mayor que 0.

Dentro de esa repetición, muestra un aviso y vuelve a solicitar y leer la cantidad.

**Comprueba:** si el usuario introduce 0, −3 y 2, solo el 2 debe aceptarse.

**Paso 6. Actualiza los totales**

Ahora el precio y las unidades son válidos.

Escribe las operaciones necesarias para:

- Añadir las unidades del producto al total de unidades.
- Añadir el coste de ese producto al importe acumulado.

Antes de escribirlas, resuelve este ejemplo a mano: llevas **4 unidades y 30 euros**, y añades **2 unidades de un producto de 5 euros**. ¿Qué deberían guardar ahora los totales?

Recuerda que debes conservar lo acumulado anteriormente.

**Paso 7. Prepara el siguiente producto**

Todavía dentro del bucle de la compra, vuelve a solicitar y leer un precio.

Comprueba de nuevo que no sea negativo, igual que hiciste en el paso 3.

Después, cierra el bucle de la compra. Al volver a comprobar su condición, el algoritmo decidirá si procesa otro producto o termina.

**Comprueba:** si el nuevo precio es 0, no debe volver a pedir unidades.

**Paso 8. Comprueba si hay compra**

Fuera del bucle, utiliza una condición para distinguir estas situaciones:

- No se ha comprado ninguna unidad: muestra «No se han registrado productos».
- Sí hay unidades: calcula el descuento y presenta el resumen.

Los pasos **9 y 10** pertenecen únicamente al segundo caso.

**Paso 9. Decide y calcula el descuento**

Guarda en una variable el porcentaje que corresponda al importe acumulado:

| Importe de la compra | Descuento |
|---|---:|
| Menos de 50 euros | 0 % |
| Desde 50 hasta menos de 100 euros | 5 % |
| Desde 100 euros | 10 % |

Utiliza condiciones para elegir el porcentaje. Después, calcula la cantidad de euros que se descuentan y el importe que queda por pagar.

Comprueba especialmente dónde entran **50 y 100 euros**.

**Paso 10. Muestra el resumen y termina**

Presenta, con mensajes claros:

- Total de unidades.
- Importe antes del descuento.
- Porcentaje aplicado.
- Descuento en euros.
- Importe final.

Cierra las condiciones pendientes y escribe el final del algoritmo. No necesitas redondear ni validar entradas de texto.

**Ejemplo de interacción**

```text
CAJA DE LA TIENDA
Introduce el precio unitario en euros (0 para terminar):
20
Introduce el número de unidades:
2
Introduce el precio unitario en euros (0 para terminar):
10
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

**Última comprobación**

Recorre tus instrucciones como si fueras el ordenador. Prueba también a introducir 0 como primer precio: debe mostrar que no hay productos, sin pedir unidades ni presentar el resumen.
