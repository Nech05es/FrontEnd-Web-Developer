# Tipos de Datos en JavaScript

### String

Estos son cadenas de texto y se declaran haciendo uso de comillas dobles o simples ( ""/'' ).
```
// JavaScript
let comillas_dobles = "This is a String";
let comillas_simples = 'This is too a String';
```
---
### Number

Estos son números Enteros y Flotantes.
```
//JavaScript
let Entero = 1000;
let Flotante = 3.1416;
```
---
### Object
Este tipo de dato es mas complejo de explicar aqui, pero aqui hay un ejemplo de como se declaran.
```
//JavaScript
let objeto = {
    propiedad_1: "Propiedad Uno",
    propiedad_2: 2
};
```
---
### Boolean
Estos son datos tipo lógico siendo (true) como algo verdadero y (false) para algo falso.
```
//JavaScript
let logico = true;
logico = false;
```
---
### Function

Este tipo de dato es complejo de explicar por lo cual solo dejare el ejemplo de declarar este tipo de dato.
```
//JavaScript
function miFuncion(){};
```
---
### Symbol

Este tipo de dato es complejo, se usa para darle un valor único a una variable.
```
//JavaScript
let simbolo = Symbol("Simbolo");
```
---
### Class
Este tipo de dato es complejo, se define como tipo de dato (function)
```
//JavaScript
class Persona{
    constructor(nombre,apellido){
        this.nombre = nombre;
        this.apellido = apellido;
  };
};
```
---
### Undefined
Este tipo de dato se asigna automáticamente en cualquier variable a la cual no se le a asignado ningún valor, también puede ser asignado manualmente.
```
//JavaScript
let x;
let y = undefined;
```
---
### Null
Este tipo de dato simboliza la ausencia de un valor y lo asignamos a una variable cuando se desea que permanezca sin valor.
```
//JavaScript
let sin_valor = null;
```
---
### Array
Este tipo de dato se cataloga como (object), este es un listado de datos al cual se le conoce como Arreglo o Array.
```
//JavaScript
let autos = ['BMW','Audi','VOLVO'];
```

---
## Typeof En JavaScript
Este operador analiza que tipo de dato se esta manejando dentro de una variable.
```
//JavaScript
console.log(typeof Entero);
console.log(typeof objeto);
console.log(typeof comillas_simples);
```
Resultado:

```
//Console
> number
> object
> string
```
---
## Concadenacion de Cadenas (Strings)
La concadenacion es la union de dos cadenas de texto haciendo uso de el operador de Adicción, de la siguiente manera.
```
let cadena1 = "Mi nombre es ";
let cadena2 = "Nestor Estrada";
console.log(cadena1 + cadena2);
console.log("Aqui no vive " + cadena2);
```
Resultado:
~~~
//Console
> Mi nombre es Nestor Estrada
> Aqui no vive Nestor Estrada
~~~