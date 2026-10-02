**Ejercicio guiado de diagrama de flujo — Acceso con intentos limitados**

Diseña un diagrama de flujo que solicite una clave numérica para permitir el acceso. La clave correcta es **2468** y el usuario dispone de un máximo de **tres intentos**.

**Requisitos**

- Cada clave introducida cuenta como un intento.
- Si la clave es correcta, muestra «Acceso permitido» y termina, aunque sea el tercer intento.
- Si es incorrecta y quedan intentos, muestra cuántos quedan y vuelve a solicitarla.
- Si falla el tercer intento, muestra «Acceso bloqueado» y termina.
- Puedes suponer que se introducen números enteros.
- Utiliza los símbolos correspondientes a inicio y fin, entrada y salida, procesos y decisiones. Etiqueta las salidas de las decisiones con «Sí» y «No».

**Ejemplo de interacción**

```text
Introduce la clave numérica:
1234
Clave incorrecta. Intentos restantes: 2
Introduce la clave numérica:
2468
Acceso permitido.
```

**Pistas para construir el diagrama**

**1. Piensa qué debes recordar**

Además de la clave correcta y la introducida, ¿qué dato necesitas para limitar las oportunidades? ¿Cuánto debe valer antes de que el usuario escriba la primera clave?

**2. Localiza las decisiones**

Debes averiguar si la clave permite entrar y si se puede volver a intentar.

Prueba este caso antes de dibujar: el usuario acierta en su tercera oportunidad. ¿Cómo organizarías las decisiones para permitirle entrar?

**3. Cuenta cada intento una sola vez**

Elige dónde actualizarás la cuenta. Sigue mentalmente una vuelta: ¿se cuenta tanto una respuesta correcta como una incorrecta?

**4. Dibuja el camino de vuelta**

Si la clave es incorrecta y quedan oportunidades, ¿a qué parte del diagrama debe regresar la flecha?

Comprueba que ese regreso no reinicie la cuenta de intentos.

**Comprueba tu diagrama**

Sigue las flechas con cuatro casos: acierto a la primera, acierto a la tercera, tres fallos y un fallo seguido de un acierto.

En todos ellos debe quedar claro cuándo se vuelve a preguntar y cuándo se termina. Nunca debe solicitarse una cuarta clave.
