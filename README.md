# Revisión JavaScript 

## Números y Cadenas
 
JavaScript puede entender diferentes tipos de datos como números y cadenas. 
Intenta escribir n número en la consola:
```
> 2
```
De forma similar. intenta escribir cualquier cadena en la consola: 

```
> "Hola Mundo"
``` 
Recuerda, las cadenas están entre comillas altas o inglesas.

## Variables

Puedes guardar datos dentro de contenedores (variables) usando "var". 

¿Puedes guardar tu nombre dentro de una variable? 
```
> var name = "Rajeev"
```
Ahora, llama a la variable para ver lo que contiene. 
```
> name
```
Puedes ver tu nombre impreso en la consola. 

Las cadenas son objetos en JavaScript y tienen algunas propiedades y funciones definidas. 

```
name.length
```
```
name.toUpperCase()
```
Podrás ver tu nombre en letras mayúsculas.

También puedes guardar cualquier número dentro de una variable. 

```
> var num = 5
```

También puedes convertir una cadena a un número:

```
parseInt("123")
```

## Operaciones aritméticas
Puedes usar operaciones aritméticas en números usando operadores aritméticos (+ , - , /, *, %).

_Nota: Recuérdale a los alumnos que el operador módulo (%) les da el remanente al dividir dos números._

Puedes intentar hacer diferentes operaciones aritméticas en la consola.
```
2+3
```
```
2-3
```
```
5*7
```
```
36/12
```
```
12%5
```
Intenta usar el operador aritmético '+' en cadenas y adivina lo que pasará:

```
"Hola" + "Amigo"
```
Las cadenas se unen cuando las sumas.

Ahora intenta usar cualquier otro operador aritmético en cadenas, como la división (/).

```
"a" / "b"
```
Obtendrás un **NaN** que significa Not A Number - No es un número. 

Ahora intenta dividir algún número entre 0: 

```
1/0
```
Obtendrás **Infinity** como respuesta. 

## Booleano (o lógico)
Hay otro tipo de dato llamado booleano en JavaScript que sólo puede contener valores **true** o **false**. 
```
var bool = true
```

Los Operadores de comparación (>,<,>=,<=,===, !=) también evalúan valores booleanos.
Intenta usar cualquiera de los operadores de comparación con números en la consola.
```
2===3
```
Esto escribirá falso en la consola. 

## Otros tipos de datos 
Hay otros dos tipos de datos en JavaScript: **null** and **undefined**

**null** es usado cuando quieres que una variable no contenga nada.
**undefined** es el valor dentro de una variable cuando has olvidado asignarle algo. 

```
var test
```
Ahora intenta ver que está dentro de 'test'.
```
test
```
## Programación condicional 
Podemos usar bloques if-else para crear programación condicional.
Intenta escribir una oración if-else sencilla:
```
if(3>2){
	console.log("Feliz")
}
else{
	console.log("No feliz")
}
```
Si la condición evalúa en **true**, el bloque es ejecutado. De lo contrario, el bloque 'else' se ejecuta.

La declaración Switch es otra forma en la que podemos hacer programación condicional. 

```
var name = "My name";

switch(name) {  
case  "My name":  
console.log("Condición 1");  
break;  
case  "my Name":  
console.log("Condición 2");  
break;  
default:  
console.log("Ninguna de las condiciones es verdadera");
}
```

## Loops (o ciclos)
A las computadoras no les gusta repetirse. Nosotros usamos ciclos para realizar una función repetitiva. Hay dos tipos de ciclos: **for** and **while**.

Escribe un ciclo **for** sencillo:

```
for(var i=0; i<=5; ++){
	console.log(i)
}
```

Escribe un ciclo **while** sencillo: 

```
var i =0
while (i<=5){
	console.log(i)
	i=i+1
}
```

## Arrays (o arreglos)
Los arreglos son un tipo de estructura de datos donde puedes usar una variable única para guardar una lista de elementos. 

Escribe un arreglo que guarde una lista de elementos. 

```
var friends = ["amigo1","amigo2","amigo3"]
```
Puedes acceder a cualquier elemento en la lista usando índices. 
_Nota: Las computadoras comienzan a contar en 0._
```
friends[0]
```

También puedes hacer ciclos dentro de los elementos usando un ciclo **for-each**.

```
for(var index in friends){
	console.log(friends[index])
}
```

Los arreglos también son objetos en JavaScript. Tienen algunas propiedades y funciones definidas. 
Por ejemplo, puedes obtener el tamaño (lenght) de un arreglo usando la propiedad 'length':

```
friends.length
```

También puedes incluir nuevos elementos en el arreglo usando push():

```
friends.push("amigo4")
```
Ahora puedes ver los elementos en el arreglo 'friends': 
```
friends
```

También puedes eliminar el último elemento del arreglo usando pop():

```
friends.pop();
```

## Funciones
Javascript tiene ciertas funciones preconstruidas que puedes usar. 
También puedes escribir tus propias funciones. 
Escribe una función para calcular la circunferencia de un círculo. Debe tomar el radio como argumento. 

```
function circumference(radius){
	var circumference = 2 * 3.14 * radius
	return circumference
}
```
Ahora puedes usar la función 'circumference' para calcular la circunferencia de cualquier círculo. 

```
circumference(5)
```

## Objetos
Usamos clases para diseñar blueprints (o plantillas) de objetos en JavaScript y luego usamos **new** para crear el nuevo objeto usando la clase. 

Internamente, JavaScript crea un nuevo objeto usando *new Object()*.
```
var paddle = new Object();
```
Puedes asignar nuevas propiedades y funciones para probar objetos. 

Pídele al alumno que asigne una nueva propiedad y función para probar un objeto. 

```
paddle.length = 60
```

```
paddle.showLength = function(){
	console.log(paddle.length);
}
```

Llama a paddle.showLength() para ver el tamaño de 'paddle'.

```
paddle.showLength()
```

Llama al objeto 'paddle' para mirar qué está guardado dentro de él. 

```
paddle
```
