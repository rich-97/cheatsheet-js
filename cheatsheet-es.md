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

## Object
```javascript

/* Declaración de objeto */

new Object([valor])                     // El constructor Object crea un contenedor de objeto.

/* Metodos de los objetos */

Object.assign(objetivo, ...fuentes)         // Copia los valores de todas la propiedades enumerables de uno o más objetos fuente a un objeto destino. Retorna el objeto destino. 
Object.create(proto [, propertiesObject ])  // Crea un nuevo objeto con el objeto y propiedades del prototipo especificado.
Object.defineProperties(obj, propiedades)   // Define nuevas o modifica propiedades existentes directamente en el objeto, returnando el objeto.
Object.defineProperty(obj, prop, descriptor)// Define una nueva propiedad sobre un objeto, o modifica una ya existente, y devuelve el objeto modificado.  
Object.freeze(obj)                          // Dongela un objeto: es decir, previene que nuevas propiedades sean agregadas; previene que las propiedades existentes sean eliminadas; y previene que las propiedades existentes, o su capacidad de enumeración, configuración, o escritura, de ser cambiadas
Object.getOwnPropertyDescriptor(obj, prop)  // Regresa como descripción de propiedad para una propiedad propia (eso es, una presente directamente en el objeto, no presente por la fuerza a través de la cadena de prototipo del objeto) de un objeto dado.
Object.getOwnPropertyNames(obj)             // Devuelve un array con todas las propiedades (numerables o no) encontradas en un objeto dado.
Object.getPrototypeOf(obj)                  // Devuelve el prototipo (es decir, el valor de la propiedad interna [[Prototype]]) del objeto especificado.
Object.isExtensible(obj)                    // Determina si un objeto es extendible (si puede tener propiedades nuevas agregadas a éste).
Object.isFrozen(obj)                        // Determina si un objeto está congelado.
Object.isSealed(obj)                        // Determina si un objeto esta sellado.
Object.keys(obj)                            // Devuelve una matriz de las propias propiedades enumerables de un objeto dado, en el mismo orden que el proporcionado por un bucle for ... in (la diferencia es que un bucle for-in enumera las propiedades de la cadena prototype como bien).
Object.preventExtensions(obj)               // Impide que se agreguen nuevas propiedades a un objeto (es decir, impide futuras extensiones al objeto).
obj.hasOwnProperty(prop)                    // Devuelve un booleano que indica si el objeto tiene la propiedad especificada como propiedad propia (no heredada).
prototypeObj.isPrototypeOf(object)          // Determina si un objeto existe en la cadena de prototipos de otro objeto.
obj.propertyIsEnumerable(prop)              // Devuelve un booleano que indica si la propiedad especificada es enumerable.
obj.toLocaleString()                        // Devuelve una cadena que representa el objeto. Este método está destinado a ser anulado por objetos derivados para propósitos específicos de la localidad.
Object.toSource()                           // Devuelve una cadena que representa el código fuente del objeto.
obj.toString()                              // Devuelve una cadena representando el objeto.
obj.unwatch(prop)                           // Elimina un conjunto de puntos de control con el método watch ().
object.valueOf()                            // Devuelve el valor primitivo del objeto especificado.
obj.watch(prop, handler)                    // Observa una propiedad a la que se le asigna un valor y ejecuta una función cuando se produce.
Object.seal(obj)                            // Sella un objeto, evitando que se agreguen nuevas propiedades y marque todas las propiedades existentes como no configurables. Los valores de las propiedades actuales se pueden cambiar siempre y cuando sean escriturables.
Object.setPrototypeOf(obj, prototype);      // Establece el prototipo (es decir, la propiedad interna [Prototype]] de un objeto especificado en otro objeto o null.
```

## String

```javascript 
/* Propiedades de la clase */

String.length                // Devuelve la longitud del arreglo.

/* Metodos de la clase */

string.fromCharCode(x)       // Devuelve una cadena creada mediante el uso de una secuencia de valores Unicode especificada.
string.fromCodePoint(x)      // Devuelve una cadena creada por una secuencia de puntos de codigo.
string.charAt(index)         // Devuelve el carácter especificado de una cadena.
string.concat(, ... StringN) // Combina el texto de uno o mas cadenas y devuelve una nueva cadena.
string.endsWith(String)      // Determina cuando una cadena termina con caracteres de una cadena especificada, retorna bool.
string.includes('string')    // Determina cuando una cadena puede encontrar otra cadena, retorna bool.
string.indexOf('string')     // Retorna el indice dentro de la llamada al objeto cadena de la primera ocurrencia del valor especifico empezando a buscar en fromIndex, retorna -1 si no se encontro.
string.lastIndexOf('string') // Retorna el indice dentro de la llamada al objeto cadena de la ultima ocurrencia del valor especifico empezando a buscar en fromIndex, retorna -1 si no se encontro.
string.match(regexp)         // Recupera en un arreglo la comparacion cuando se comparo la cadena con la expresion regular.
string.repeat(number)        // Construye y devuelve una nueva cadena que contiene el numero especifico de repeticiones del arreglo llamado concatenado.
string.search(regexp)        // Ejecuta una busqueda por una comparacion regular en un objeto string.
string.slice(index, end)     // Extrae una seccion de una cadena y retorna una nueva cadena.
string.split(separator)      // Divide un objeto de cadena en un arreglo de cadenas separados en subcadenas.
string.toLowerCase('string') // Coloca los caracteres en minuscula.
string.toUpperCase('string') // Coloca los caracteres en mayuscula.
string.trim('string')        // Quita los espacios en blanco de una cadena.
string.substr(start,length)  // Retorna los caracteres en una cadena empezando por el inicio de una localizacion especificada por el numero de caracteres.
```

## Function

```javascript
/* Metodos de una función */

function.apply(thisArg, array) // invoca una determinada función asignando explícitamente el objeto this y un array o similar  como parámetros (argumentos) para dicha función.
function.bind(thisArg) // es un método del objeto Function creado para manipular el valor contextual de this. 
function.call(thisArg, args...) // El método call() llama a una función con un valor this asignado y argumentos provistos de forma individual.
function.isGenerator() // El método isGenerator() determina si una función es un generador. 
function.toSource() // devuelve un string representando el código fuente del objeto.
function.toString() // retorna una cadena representando el código fuente de la función.
```
