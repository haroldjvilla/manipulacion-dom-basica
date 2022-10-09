## Respuestas al Test de JavaScript

Recuerda que estas respuestas (o al  menos la mayoría) NO SON ABSOLUTAS. Es completamente válido (en la mayoría de casos) si tienes otras respuestas. Recuerda que podemos discutirlo en la sección de comentarios del curso. :D


## Variables y operaciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una variable y para qué sirve?
//Espacions en memoria de los diferentes tipos de datps

- ¿Cuál es la diferencia entre declarar e inicializar una variable?
//Declarar es cuan le decimios a javaScript que vamos a crear una variable con el nombre tal. Mientreas que inicializar es asignarle un valor a esa variable.

- ¿Cuál es la diferencia entre sumar números y concatenar strings?

- ¿Cuál operador me permite sumar o concatenar?
// el operador es + Esto nos permirte hacer operaciones matematicas de suma con numeros, pero con strings, lo que hace es unir los strings

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre    //string
- Apellido   //string
- Nombre de usuario en Platzi   //string
- Edad  //number
- Correo electrónico  //string
- Mayor de edad  //boolean
- Dinero ahorrado   //number
- Deudas  //number

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

let nombre = "Harold";
let apellido = "Jaramillo";
let edad = 31;
let correoElectronico = "haroldvilla22@gmail.com";
let isMayorDeEdad = true;
let dineroAhorrado = 10;
let deudas = 3;

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)
- Dinero real (dinero ahorrado menos deudas)

let nombreCompleto = nombre + (" ") +apellido;
let dineroReal = dineroAhorrado - deudas;


## Funciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una función?

//Las funciones nos permite guardar bloques de codigo para reutilizarlos y ademas ejecutarlos en el futuro.


- ¿Cuándo me sirve usar una función en mi código?

//Nos sirve cuando tenemos bloques de codigo completo muy parecidos que podemos encapsular para reutilizar más de una vez en el futuro.

Tambian nos sirve para ordenar y mejorar la legibilidad de nuestro código.

- ¿Cuál es la diferencia entre parámetros y argumentos de una función?

// Las funciones reciben parámetros cuando las creamos. Y les enviamos argumentos cuando las ejecutamos.

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```
 
```


function nombreCompleto(name, lastName) {
    return name + ' ' + lastName
}

function saludo(name, lastMame, userName) {
    const completeName = nombreCompleto(name, lastName);

    console.log("Mi nombre es " + comleteName + ", pero prefiero que me digas " + userName + ".");
}

## Condicionales

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un condicional?

//Son la forma en que ejecutamos un bloque de código u otro dependiendo de alguna condicón o validación.

- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?

// if(elsey else if), Switch

El condicional if (con else y else if) nos permite hacer validaciones completamente distintas ( se asi queremos) en cada validación o condicional. El cambio, en el switch todos los cases se comparan con la misma variable o condición que definimos en el switch.

- ¿Puedo combinar funciones y condicionales?

Sí. las funciones pueden encapsular cualquier bloque de código, incluyendo condicionales.

### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

```
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;
   case "ExpertDuo":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
       break;
}
```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

> 💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays y un solo condicional. 😏


## Ciclos

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo?

//La forma de ejecutar un bloque de código hasta que se cumpla cierta condición.
La forma de ejecutar un bloque de código mientras una condición sea verdadera o se cumpla


- ¿Qué tipos de ciclos existen en JavaScript?

// While, do while y for.

- ¿Qué es un ciclo infinito y por qué es un problema?

//Es cuando la validación de nuestros condicionakes nunca se cumple y termina toteando (Dañada) la aplicación (e.j. cuando lel navegador ya no puede más de tanta ejecución de ese bloque de código).

- ¿Puedo mezclar ciclos y condicionales?


Sí, aunque los ciclos son una especie de condicionales, nada nos uimpide agregar más condicionales dentro del ciclo.

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

while (i < 5) {
    console.log("El valor de i es : " + i);
    i++;
}



for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}

while (i >=2 ) {
    console.log("El valor de i es : " + i);
    i--;
}

```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es `2 + 2`. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

> 💡 Pista: puedes usar la función prompt de JavaScript.


//
while (respuesta != "4") {
    let pregunta = prompt("¿Cúanto es 2 + 2?")
    respuesta = pregunta;
}

## Listas

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un array?

//Es una lista de elementos.

'''
const array = [1, 'jaja', true, false];
'''

- ¿Qué es un objeto?

es una lista de elementos PERO cada elemento tiene un numbre clave.

const obj = {
    nombre: 'Fulanito',
    edad: 3,
};

- ¿Cuándo es mejor usar objetos o arrays?

Arrays cuando lo que haremos en un elemento es lo  mismo que en todos los demás (la regla se puede incumplir). Mientras que un objeto cuando los nombres de cada elemento son importantes para nuestro algoritmo.

- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?


Sí. los arrays pueden guardar objetos y los objetos pueden guardar arrays entre sus propiedades

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

let arr = ['maria', 'carlos', 'rosa', 'juan'];

function imprimirElemento(array) {
    console.log("Primer elemen:",arr [0])
}

imprimirElemento()

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

function imprimirElementoPorElemento(array) {

    for (let index = 0; index < arr.length; index++) {
        const element = arr[index];
        
        console.log(element)   
    }
}

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).


function imprimirElementoDeObjeto(obj) {
    const arr = Object.values(obj);
    for (let index = 0; index < arr.length; index++) {
        
        console.log(arr[index])   
    }
};