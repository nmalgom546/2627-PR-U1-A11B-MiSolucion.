**Diagrama de flujo guiado paso a paso — Acceso con intentos limitados**

Vas a dibujar un sistema de acceso con la clave numérica **2468**. El usuario tendrá un máximo de **tres intentos**.

Si acierta, podrá entrar. Si falla las tres veces, el acceso quedará bloqueado.

**Paso 1. Dibuja el inicio y prepara los datos**

Dibuja el símbolo de inicio.

Después, añade un rectángulo para preparar la clave correcta y un contador de intentos. Piensa cuánto debe valer el contador cuando todavía no se ha introducido ninguna clave.

**Paso 2. Solicita la clave**

Añade los símbolos de entrada y salida necesarios para:

1. Mostrar «Introduce la clave numérica».
2. Leer la respuesta del usuario.

Conéctalos en ese orden.

**Paso 3. Cuenta el intento**

Añade un rectángulo para actualizar el contador: acaba de introducirse una clave y eso cuenta como un intento.

Piensa qué operación permite aumentar la cuenta en uno.

**Paso 4. Comprueba si la clave es correcta**

Dibuja un rombo que compare la clave introducida con la correcta.

Traza dos salidas, etiquetadas como «Sí» y «No»:

- Por «Sí», muestra «Acceso permitido» y conduce al final.
- Por «No», continúa con el siguiente paso.

**Paso 5. Comprueba si quedan oportunidades**

En el camino de la clave incorrecta, dibuja otro rombo para decidir si todavía quedan intentos disponibles.

Recuerda que solo se permiten tres. Escribe una condición que distinga entre **haber usado menos de tres** y **haberlos agotado**.

**Paso 6. Dibuja el camino para volver a intentarlo**

Si quedan oportunidades:

1. Calcula cuántas quedan.
2. Muestra «Clave incorrecta» y la cantidad de intentos restantes.
3. Dibuja una flecha que regrese a la petición de la clave.

La flecha debe volver al **paso 2**. Si volviera a preparar el contador, se perderían los intentos realizados.

**Paso 7. Dibuja el camino de bloqueo**

Si ya no quedan oportunidades, muestra «Acceso bloqueado» y conduce al final.

Desde este camino no debe poder solicitarse otra clave.

**Ejemplo de interacción**

```text
Introduce la clave numérica:
1111
Clave incorrecta. Intentos restantes: 2
Introduce la clave numérica:
2222
Clave incorrecta. Intentos restantes: 1
Introduce la clave numérica:
2468
Acceso permitido.
```

**Paso 8. Comprueba el dibujo siguiendo las flechas**

Utiliza un dedo o un lápiz para recorrer el diagrama y anota el contador en cada intento.

Comprueba estos tres casos:

- Aciertas a la primera: permite el acceso y termina.
- Fallas dos veces y aciertas a la tercera: también permite el acceso.
- Fallas tres veces: bloquea el acceso y no solicita una cuarta clave.

Revisa que todos los caminos lleguen a su destino y que cada rombo tenga sus salidas «Sí» y «No».
