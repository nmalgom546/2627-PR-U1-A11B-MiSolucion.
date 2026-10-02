**Ejercicio de diagrama de flujo — Acceso con intentos limitados**

Diseña un diagrama de flujo que solicite una clave numérica para permitir el acceso. La clave correcta es **2468** y el usuario dispone de un máximo de **tres intentos**.

**Requisitos**

- Solicita una clave numérica y comprueba si es correcta.
- Cada clave introducida cuenta como un intento.
- Si la clave es correcta, muestra «Acceso permitido» y termina inmediatamente.
- Si es incorrecta y quedan intentos, muestra cuántos quedan y vuelve a solicitarla.
- Si falla el tercer intento, muestra «Acceso bloqueado» y termina.
- Puedes suponer que el usuario introduce números enteros.
- Representa el inicio y el fin, las entradas y salidas, los procesos y las decisiones con sus símbolos correspondientes. Identifica las salidas de cada decisión con «Sí» y «No».

**Ejemplo de interacción: acierto en el segundo intento**

```text
Introduce la clave numérica:
1234
Clave incorrecta. Intentos restantes: 2
Introduce la clave numérica:
2468
Acceso permitido.
```

**Ejemplo de interacción: intentos agotados**

```text
Introduce la clave numérica:
1111
Clave incorrecta. Intentos restantes: 2
Introduce la clave numérica:
2222
Clave incorrecta. Intentos restantes: 1
Introduce la clave numérica:
3333
Acceso bloqueado.
```
