# [Documentación](https://es.javascript.info/)

## Variables
Hay tres formas de declarar variables en JS

```javascript
// Declarar una variable con var
var x = 5;

// Declarar una variable con let
let y = "Hola";

// Declarar una constante
const PI = 3.14159;

```

## Operadores
### Aritméticos
	- Sumar -> +
	- Restar -> - 
	- Multiplicar -> *
	- Dividir -> /

### Comparación
	- Igual en contenido -> ==
	- Igual el tipo y contenido -> ===
	- No es igual en contenido -> !=
	- No es igual en tipo y contenido -> !==
	- Menor que -> <
	- Mayor que -> >
	- Menor o igual que -> <=
	- Mayor o igual que -> >=

### Lógicos
	- AND -> &&
	- OR -> ||
	- NOT -> !

### Asignación
	- Asignar un valor -> =
	- Suma y asigna -> += <- Tambien concatena y asigna
	- Resta y asigna -> -=
	- Multipilca y asigna -> *=
	- Divide y asigna -> /=


## Estructuras de control
Sentencias para el controlar le flujo del programa.

### if
Se utiliza para ejecutar un bloque **si** se cumple una determinada condición.
```javascript
if (condición) {
	// Código a ejecutar si la condición es verdadera
} else {

}
```

### else if
Se utiliza en conjuto con if, para crear una estructura de control con varias condiciones consecutivas.
```javascript
if (condición1) {
  // Código a ejecutar si la condición1 es verdadera
} else if (condición2) {
  // Código a ejecutar si la condición2 es verdadera
} else {
  // Código a ejecutar si todas las condiciones anteriores son falsas
}
```

### while
Se utiliza para ejecutar diferentes bloques de código dependiendo del valor de una expresión.
```javascript
switch (expresión) {
  case valor1:
    // Código a ejecutar si la expresión es igual a valor1
    break;
  case valor2:
    // Código a ejecutar si la expresión es igual a valor2
    break;
  // ...
  default:
    // Código a ejecutar si la expresión no es igual a ninguno de los valores anteriores
}
```

### while
Se utiliza para crear un bucle que se ejecuta mientras una determinada condición se cumpla.
```javascript
while (condición) {
  // Código a ejecutar mientras la condición sea verdadera
}
```

### do-while
Es similar al while, pero con la diferencia clave de que el bloque dentro de las llaves se ejecuta **al menos una vez**.
```javascript
do {
  // Código a ejecutar al menos una vez
} while (condición);
```

### for
Sirve para crear un bucle que se ejecuta un número específico de veces.
```javascript
for (inicialización; condición; expresión de iteración) {
  // Código a ejecutar en cada iteración
}
```

## Funciones
Son bloques de código que pueden ser llamados en cualquier momento del programa y se utilizan para realizar tareas especificas.

```javascript
function nombreFuncion(parametro1, parametro2, ...) {
  // Código a ejecutar
  return valorDeRetorno;
}
```

Donde: 
-   `nombreFuncion`: es el nombre que se le da a la función.
-   `parametro1`, `parametro2`, ...: son los parámetros de entrada de la función. Estos son opcionales y se utilizan para pasar valores a la función para que los procese.
-   `// Código a ejecutar`: es el bloque de código que contiene las instrucciones que la función debe ejecutar.
-   `return valorDeRetorno;`: es una sentencia opcional que indica el valor que la función debe devolver al final de su ejecución.

## Objetos
Son estructuras de datos que contienen propiedades y métodos. Son fundamentales para la programación orientada a objetos. Se permiten agrupar valores y funciones en una sola entidad.

```javascript
var objeto = {
  propiedad1: valor1,
  propiedad2: valor2,
  metodo1: function() {
    // Código a ejecutar
  },
  metodo2: function() {
    // Código a ejecutar
  }
};
```

Donde:

-   `objeto`: es el nombre que se le da al objeto.
-   `propiedad1`, `propiedad2`: son las propiedades del objeto. Cada propiedad se define utilizando un nombre y un valor separados por dos puntos. El valor puede ser cualquier tipo de dato válido en JavaScript, incluyendo otros objetos y funciones.
-   `metodo1`, `metodo2`: son los métodos del objeto. Cada método es una función que se define de la misma manera que las funciones normales.

Para acceder a las propiedades o métodos de un objeto:

```javascript
objeto.propiedad; // Acceder a una propiedad
objeto.metodo(); // Llamar a un método
```

## Eventos
Son acciones que suceden en una página web, como hacer clic en un botón. Permite a los programadores capturar estos eventos y realizar acciones especificas en respuesta ellos.

Los eventos se manejan mediante event listeners *(escuchadores)*. Es una función que se ejecuta cuando ocurre un evento especifico en la página.

```javascript
elemento.addEventListener(evento, funcion);
```

Donde:

-   `elemento`: es el elemento HTML al que se agrega el event listener.
-   `evento`: es el nombre del evento al que se quiere responder, por ejemplo, "click", "mouseover", "submit", etc.
-   `funcion`: es la función que se ejecuta cuando ocurre el evento.

Los más usados:
1.  `click`: Se activa cuando el usuario hace clic en un elemento.
2.  `submit`: Se activa cuando el usuario envía un formulario.
3.  `mouseover`: Se activa cuando el usuario mueve el ratón sobre un elemento.
4.  `keydown`: Se activa cuando el usuario presiona una tecla del teclado.
5.  `load`: Se activa cuando se ha cargado completamente una página web.
6.  `unload`: Se activa cuando se descarga una página web o se navega lejos de ella.
7.  `resize`: Se activa cuando el tamaño de la ventana del navegador cambia.
8.  `scroll`: Se activa cuando el usuario desplaza la página hacia arriba o hacia abajo.

