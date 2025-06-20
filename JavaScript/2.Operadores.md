# Operadores en JavaScript
## Operadores Aritméticos
Estos operadores permiten hacer operaciones matemáticas.
#### Operador De Adición (+)
Este operador Suma dos valores.
```
let a = 2, b = 3;
console.log( a + b );
```
#### Operador de Sustracción (-)
Este operador resta dos valores.
```
let a = 2, b = 3;
console.log( a - b );
```
#### Operador de Multiplicación (*)
Este operador multiplica dos valores.
```
let a = 2, b = 3;
console.log( a * b );
```
#### Operador Exponente (**)
Este operador multiplica el valor por una cantidad de veces.
```
let a = 2, b = 3;
console.log( a ** b );
```
#### Operador de División (/)
Este operador divide dos valores.
```
let a = 4, b = 2;
console.log( a / b );
```
#### Operador de Modulo (%)
Este operador divide dos valores y regresa el valor restante.
```
let a = 4, b = 2;
console.log( a % b );
```
---
## Operadores de Incremento y Decremento.
### Incremento (++)
Este operador incrementa el valor de una variable una vez.
#### Pre-Incremento
El pre-incremento incrementa primero el valor de la variable y luego podemos almacenarlo en una variable.
```
let numero = 1;
let incremento = ++numero;
console.log(incremento);
```
#### Pos-incremento
El pos-incremento primero almacena el valor y después lo incrementa, y este incrementa no se vera reflejado hasta la próxima vez que utilizamos el valor.
```
let numero = 1;
let incremento = numero++;
console.log(incremento);
```
>! (Nota) Tanto [pre] y [pos] Decremento (--) funcionan de igual manera que Incremento, simplemente este resta un valor en ves de aumentarlo.
---
## Precedencia de Operadores Aritméticos

La precedencia de operadores es el orden que sigue el compilador para hacer las operaciones matemáticas.

1. Paréntesis (  )
2. Exponencial **
3. Multiplicación *
4. Divicion /
5. Modulo %
6. Adicción +
7. Sustracción -
---

## Operadores de Asignacion (=)
El operador de asignacion (=) lo hemos estado usando al declarar variables y asignarles un valor.
```
let variable = 10;
```
##### Operadores de asignacion compuestos
Esto aplica en dos operadores [+=] [-=] incremento y asignacion, decremento y asignacion.
###### Incremento y Asignacion
```
variable += 1;
console.log(variable);
```
###### Decremento y Asignacion
```
variable -= 2;
console.log(variable);
```
---
## Operadores de Comparacion
Estos operadores comparan dos expreciones y devuelven un resultado booleano.
#### Operador de Igualdad (==)
Este operador evalua si dos expreciones son iguales.
```
let a = 2, b = 3, c = '2';
console.log( a == b );
console.log( a == c );
```
> (true) son iguales.
(false) son diferentes.
(!) Operador [Estricto Igual] (===) compara si las dos expreciones son iguales tanto en el valor como en el tipo de dato.
#### Operador Diferente A (!=)
Este operador compara si las dos expreciones son diferentes.
```
let a = true, b = 5, c = 'true';
console.log( a != b );
console.log( a != c );
```
> (true) son diferentes.
(false) son iguales.
(!) Operador [Estricto Diferente] (!==) evalua si las dos expreciones son diferentes tanto en el tipo de dato como en el valor.
---
## Operadores Relacionales
Estos operadores evualuan el tamaño de dos expreciones.
#### Operador Menor A (<)
Este operador compara si una exprecion es menor a la otra.
```
let a = 2, b = 3, c = 2;
console.log( a < b );
```
>(true) Menor.
(false) Mayor.
#### Operador Menor Igual (<=)
Este operador compara si la exprecion es menor o igual a la otra.
```
let a = 2, b = 3, c = 2;
console.log( a <= c );
```
>(true) Menor o Igual
(false) Mayor
#### Operador Mayor A (>)
Este operador compara si la exprecion es mayor a la otra.
```
let a = 2, b = 3, c = 4;
console.log( b > c );
```
>(true) Mayor.
(false) Menor.
#### Operador Mayor Igual (>=)
Este operador compara si la exprecion es mayor o igual a la otra.
```
let a = 5, b = 2, c = 4
console.log( a >= c );
```
>(true) Mayor o Igual.
(false) Menor.
---
## Operadores Logicos
Estos operadores evaluan dos comparaciones y regresan un valor boolean.
#### Operador AND (&&)
Este operador compara si dos comparaciones son (true).
```
let a = true, b = false;
let and = a == b && b != a;
console.log(and)
```
>(true) Ambas comparaciones son (true)
(false) Una o ambas comparaciones son (false)
#### Operador OR (||)
Este operador compara entre dos comparaciones si una de esas es (true).
```
let a = true, b = false;
let and = a == b || b != a;
console.log(and)
```
>(true) Una o ambas comparaciones son (true)
(false) Si ambas comparaciones son (false)
---
## Operador Ternario
Este operador compara una exprecion y dependiendo el resultado booleano regresa un valor pre-definido.
```
let ternario = (1 > 2)? "true":"false"
console.log(ternario);
```
> Dependiendo del resultado de la comparacion devuelve el resultado que predefinimos despues del operador (?) ternario. Si fue (true) devuelve el primer resultado, si fue (false) devuelve el segundo resultado que esta definido despues de los dos puntos (:)
---
#### ( ! ) Combertir un Numero a String
Muchos de los datos que obtenemos del usuario en JavaScript son de tipo (String). Incluso los numeros para poder manejarlos necesitamos combertirlos a numeros.
```
let usuario = "20"
let numero = Number(usuario)
console.log(typeof usuario);
console.log(typeof numero);
```
>La funcion o metodo [Number()] combierte los numeros tipo string a number
---
## Funcion isNaN
La funcion isNaN() cuestiona si al combertir un numero-string con la funcion Number() realmente es un numero.
```
let numero_string = '18x';
let numero = Number(numero_string);
console.log(isNaN(numero));
```
>Devolviendo (true) cuando una variable no contenga un numero realmente, y false cuando si es un numero real.
