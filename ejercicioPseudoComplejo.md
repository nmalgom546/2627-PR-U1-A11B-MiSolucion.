**Ejercicio de pseudocódigo — Caja de una tienda**

Diseña un algoritmo que gestione el cobro de una compra formada por varios productos. Para cada producto se introducirá su precio unitario y la cantidad de unidades compradas. La compra terminará al introducir un precio de **0**.

**Requisitos**

- Utiliza únicamente las primitivas y los operadores estudiados.
- Solicita el precio unitario de cada producto. Si es negativo, muestra un aviso y vuelve a pedirlo hasta recibir un valor válido.
- Si el precio es 0, termina la introducción de productos **sin solicitar unidades**.
- Para cada precio positivo, solicita una cantidad entera de unidades mayor que 0. Si no es válida, muestra un aviso y vuelve a pedirla.
- Acumula el importe de la compra y el número total de unidades.
- Al terminar, aplica un descuento según el importe acumulado:
  - Menos de 50 euros: sin descuento.
  - Desde 50 euros hasta menos de 100 euros: **5 %**.
  - A partir de 100 euros: **10 %**.
- Muestra el total de unidades, el importe antes del descuento, el porcentaje aplicado, el descuento en euros y el importe final.
- Si el primer precio introducido es 0, muestra únicamente «No se han registrado productos» y termina.
- No necesitas validar entradas de texto ni redondear los resultados.

**Ejemplo de interacción**

En este ejemplo, la compra contiene dos unidades de un producto de 20 euros y tres unidades de otro de 10 euros.

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

**Otro ejemplo: compra vacía**

```text
CAJA DE LA TIENDA

Introduce el precio unitario en euros (0 para terminar):
0
No se han registrado productos.
```
