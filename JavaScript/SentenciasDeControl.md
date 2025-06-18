# Sentencias de Control en JavaScript
Las sentencias de control revisan una expresion Boolean y dependiendo del resultado se ejecuta un bloque de codigo.
### Sentencia IF
Esta sentencia resive la expresion boolean y si la expresion retorna (true) se ejecuta el bloque de codigo que esta declarado dentro de esta sentencia.
```
if(true === true){
    console.log('La expresion retorna (true)');
}
```
### Sentencia ELSE
Esta sentencia se ejecuta cuando la expresion en la  sentencia (if) retorna (false), entonces ejecuta el bloque declarado dentro de la sentencia (else).
```
if (true === false){
    console.log('La expresion retorna (true) ');
}else{
    console.log('La expresion retorna (false)');
}
```
### Sentencia ELSE IF
Esta sentencia actua de la misma forma que (if), la diferencia es que esta se tiene que declarar despues de la sentencia if y esta sentencia la podemos declara mas de una vez en el mismo bloque de sentencias.
```
if(false){
    continue;
}
else if(true){
    console.log('La expresion retorna (true)')
}else{
    continue;
}
```
### Ejercicio Calculo Estacion del Año
Calcula la estacion del año por el mes.
```
let mes = 4;
let estacion;
if (mes == 1 || mes == 2 || mes == 12){
    estacion = 'Invierno'
}
else if (mes == 3 || mes == 4 || mes == 5){
    estacion = 'Primavera';
}
else if(mes == 6 || mes == 7 || mes == 8){
    estacion = 'Verano';
}
else if(mes == 9 || mes == 10 || mes == 11){
    estacion = 'Otoño';
}
else{
    estacion = 'Valor incorrecto!';
}
console.log(estacion)
```
### Sentencia Switch
La sentencia switch analiza una expresion de cualquier valor y dependiendo del (caso) que con el que coincida se ejecutara un bloque de codigo que este declarado en ese (caso), de caso contrario se ejecutara un bloque de codigo que definimos como (default).
```
let boolean = true;
switch(boolean){
    case true:
        console.log('Ejecuta una accion.');
        break;
    case false:
        cosole.log('Ejecuta una accion');
        break;
    default:
        console.log('Esto se ejecuta por defualt')
}
```
>(!) Es necesario el uso de el operador (break) para finalizar cualquier ejecucion de algun bloque (case), pero el bloque (default) no es necesario agregar al final un (break) para terminar la ejecucion del bloque ya que este mismo es el final de la estructura (switch).