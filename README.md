# JavaScript
JavaScript es un lenguaje de programación de alto nivel interpretado de lado del cliente.

> Los programas en JavaScript son llamados _scripts_. Dichos scripts no necesitan preparación especial o compilación para correr.

Los navegadores web tienen un programa especial llamado **motor de JavaScript** y este motor es el que se encarga de:
1. El motor (si es un navegador) lee ("analiza") el script.
2. Luego convierte ("compila") el script al lenguaje de máquina.
3. Y luego se ejecuta el código de la máquina, bastante rápido.

Diferentes motores tienen diferentes nombres en clave, por ejemplo:
- **V8** - en Chrome y Opera.
- **SpiderMonkey** - en Firefox.


# Historia
JavaScript fue inventado por Brendan Eich en 1995. Inicialmente se llamaba **LiveScript**, pero debido a que el lenguaje de programación **Java** era muy popular en ese momento, se decidió cambiar el nombre a **JavaScript**. 


# Comentarios
Es una o varias lineas de texto en el código el cual el compilador y/o intérprete ignora. Normalmente los comentarios se utilizan para poner aclaraciones del código y también suelen ser utilizados para anular parte de un código.
```javascript
// Comentario en una sola linea
```
```javascript
/* Comentario en varias lineas */
```


# Variables
Una variable es un contenedor el cual almacena información. Técnicamente hablando, es un contenedor para almacenar valores de datos.
```javascript
var nombre = "Alfredo";
```
> * **var** es la palabra reservada.
> * **nombre** es el identificador.
> * **=** asigna un valor a una variable. 
> * **Alfredo** es el valor.

En JavaScript, existen 3 formas de declarar una variable;
```javascript
var
let
const
```

> let y const fueron introducidas por ECMAScript 2015. Estas dos palabras reservadas proporcionan variables de ámbito bloque.

# var vs. let
**Ejemplo 1**
```javascript
-------------------
{                 
  var numero = 10; 
}
// numero puede usarse aquí
-------------------

-------------------
{                 
  let numero = 10; 
}
// numero no puede usarse aquí
-------------------
```

**Ejemplo 2**
```javascript
var numero = 10; //10
{
  var numero = 2; //2
}
//2
```

```javascript
var numero = 10; //10
{
  let numero = 2; //2
}
//10
```


# Scope
El scope en JavaScript, es el alcance que tienen las variables en JavaScript. En JavaScript hay dos tipos de alcance;
* Local Scope   
* Global Scope  

El alcance determina la accesibilidad de las variables. Las variables definidas dentro de una función no son **accesibles** desde fuera de la función. Las variables declaradas de una función JS se convierten en locales a la función y únicamente se puede acceder a ellas desde dentro de la función y una variable declarada fuera de una función se convierte en global.


# Modo estricto
JavaScript tiene un modo estricto (_nuevo en ECMAScript 5_) y su sintáxis es la siguiente;
```javascript
"use strict"
```

> * No es una declaración sino una expresión literal (_ignorada por versiones anteriores de JS_).
> * Todos los navegadores modernos admiten este modo, excepto Internet Explorer 9 para abajo.
> * Podemos declararlo al comienzo de un script o dentro de una función.
> * Declarado al comienzo de un script tiene **alcance global** (_todo el script se ejecutará en modo estricto_).
> * Declarado dentro de una función tiene **alcance local** a la función (_sólo el script dentro de la función se ejecutará en modo estricto_).

**Ejemplo**
```javascript
a = 2;
console.log(a); //Muestra el valor de "a" en la cosola
```

```javascript
"use strict"
a = 2;
console.log(a); //Muestra un error en la consola porque "a" no está definida
```

El uso del modo estricto en JavaScript podría considerarse buena práctica de programación, ya que nos ayudará a estar siempre definiendo las variables.


# Fuentes
- https://javascript.info/
- https://www.w3schools.com/js/default.asp
