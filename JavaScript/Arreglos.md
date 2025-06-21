# Arrays en JavaScript
Un array alamacena una cantidad de datos que se declaran 
dentro de este array, Existen algunas formas de declarar arrays.
###### Forma deprecada
```
let Auto = new Array('Honda','Nissan','Toyota');
```
###### Forma actual y recomendada
```
const Autos = ['Honda','Nissan','Toyota'];
```
>(!) Se puede almacenar cualquier tipo de dato juntos dentro de un array.
### Acceder a datos
Al almacenar los datos los asocia con identificadores para poder acceder a los valores que se almacenan. Empezando por el numero (0) y terminando por el ultimo dato que se ha agregado. Entonces para acceder llamamos al array y dentro corchetes el id.
```
console.log(Autos[1]);
```
### Iterar un Array
Podemos recorrer un array usando un ciclo (for) de la siguiente manera.
```
for(let i = 0; i < Autos.lenght; i++){
    console.log(Autos[i])
}
```
>(!) El metodo .lenght cualcula la cantidad de datos que se encuentran dentro de el Array
### Modificar datos.
Para modificar datos de una array debemos acceder al id y declara el valor a modificar.
```
Autos[1] = 'Mitsubishi';
console.log(Autos);
```
### Agregar datos.
Hay varias formas de agregar nuevos elementos a un array, de un lado podemos usar lo largo de la lista para agregar el elemento y por otro lado tenemos el metodo .push() que nos permite hacer lo mismo.
###### Usar .length
```
Autos[Autos.length] = 'Nissan';
console.log()
```
###### Usar .push()
```
Autos.push('Subaru');
console.log(Autos);
```
##### Jumping ID
Si llegamos a almacenar un elemento saltandonos un id este automaticamente se asociara con un (string) vacio.
```
Autos[Autos.length + 1] = 'Ford';
console.log(Autos);
```
### Asking if is Array
En ocasiones en el ambito de la programacion necesitaremos saber si en una variable contienen un (array) y muy bien pudieramos usar (typeof) pero este solo devolveria (object). Asi que hay 2 maneras de saber esto.
###### Array.isArray()
```
console.log(Array.isArray(Autos));
```
###### instanceof
```
console.log(Autos instanceof Array);
```
>(!) Ambos actuan de la misma manera. Devuelven (true) si es un array y (false) si no lo es.