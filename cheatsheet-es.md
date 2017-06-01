## Math

```javascript

/* Constantes */

Math.E       // número de Euler.
Math.PI      // número pi.
Math.SQRT2   // Raíz cuadrada de 2.
Math.SQRT1_2 // Raíz cuadrada de 1 / 2.
Math.LN2     // logaritmo natural de 2.
Math.LN10    // logaritmo natural de 10.
Math.LOG2E   // logaritmo de e en base a 2.
Math.LOG10E  // logaritmo de e en base a 10.

/* Constantes arbitrarias */

Math.PI2 = Math.PI * 2
Math.PI_2 = Math.PI / 2

/* Metodos */

Math.sqrt(x)     // Devuelve la Raíz cuadrada de un número.
Math.abs(x)      // Devuele el Valor absoluto de un número.
Math.pow(x, exp) // Devuelve el número Elevado a un exponente.
Math.floor(x)    // Redondeo hacia abajo a el entero más proximo.
Math.ceil(x)     // Redondeo hacia arriba a el entero más proximo.
Math.round(x)    // Redondeo a el entero más proximo.
Math.sin(x)      // Deveulve el seno de un número (En radianes).
Math.tan(x)      // Devuelve la tangente de un número (En radianes.)
Math.cos(x)      // Devuelve el coseno de un número (En radianes).
Math.asin(x)     // Devuelve el arcoseno de un número (En radianes).
Math.acos(x)     // Devuelve el arcocoseno de un número (En radianes).
Math.atan(x)     // Devuelve el arcotangente de un número (En radianes).
Math.exp(x)      // Devuelve el valor de elevar `e` a la n.
Math.max(x, y)   // Devuelve el valor maximo de una lista de números.
Math.min(x, y)   // Devuelve el valor minimo de una lista de números.
Math.random()    // Devuelve un número aleatoria entre 0 y 1.
Math.log(x)      // Devuelve el logaritmo natural de (Base `e`) de un número.
Math.log10(x)    // Devuelve el logaritmo de un número en base a 10.

/* Algunas funciones utiles */

Math.randomInt = function (min, max) {
    return (Math.random() * (max - min) + min)
}
```

## Number

```javascript

/* Constantes de la clase */

Number.EPSILON           // Constante Epsilon.
Number.MAX_VALUE         // 1.7976931348623157e+308.
Number.MIN_VALUE         // 5e-324.
Number.NEGATIVE_INFINITY // -Infinity.
Number.POSITIVE_INFINITY // Infinity.
Number.MAX_SAFE_INTEGER  // 9007199254740991.
Number.MIN_SAFE_INTEGER  // -9007199254740991.
Number.NaN               // Not a Number (No es un número).

/* Metodos de la clase */

Number.isFinite(x)      // Retorna verdadero si el númeor es finito.
Number.isNaN(2)         // Retorna verdadero si no es un número.
Number.isInteger(2)     // Retorna verdadero si el número es un entero.
Number.isSafeInteger(2) // Retorna verdadero si el número es un entero seguro.

/* Metodos de las instancias */

x.toExponential(y)        // Devuelve una cadena Representando el número elevado a un exp.
x.toFixed(y)              // Devuelve una cadena Representando el número con una notacion de punto fijo.
x.toLocaleString('en-IN') // Devuelve una cadena Representando el número acorde al idioma.
x.toPresicion(n)          // Devuelve una cadena Representando el número según la presición (n decimales).
x.valueOf()               // Devuelve el valor primitivo del objeto.
x.toString(2)             // Devuelve una cadena representando el número en la base especificada, la base puede ser un entero entre 2 y 36.
```
