# JavaScript

## Condiciones

### Estructura de control

Una estructura de control es aquel mecanismo que permite controlar el flujo de tu programación

Dentro de las estructuras de control existen las:

 **Estructuras secuenciales** que son las que van una detras de la otra

 **Estructuras condicionales** que dependiendo de la evaluacion de una condición hacemos ciertas acciones u otras

 **Loops o estructuras repetitivas** 

 
 Ahorita lo vamos a ver, es la estructura condicional, la cual es la que se ve frecuentemente.

 ```
let edad = 17;

    if (edad > 17) {
      console.log("Eres mayor de edad");      
    } else {
      console.log("Eres menor de edad");      
    }

 if (edad >= 18) {
  console.log("Eres mayor de edad");      
} else {
  console.log("Eres menor de edad");      
}
 ```

 Donde la primera opcion, utilizamos una condicional sola. En la segunda, utilizamos condicional acompañada.En esta caso, el igual en la mayor que, tenemos que agregar el valor de la condicion. Es decir, tenemos que agregar el valor junto con la condicion.

 Cuando tenemos operadores opuestos, tenemos que colocar un valor diferente al que tenemos al valor de nuestra variable; ya que significa que estas incluyendo tambien ese valor a la variable.

 ### Condicional anidado

 Las condicionales anidadas, son cuando tenemos mas de dos opciones en nuestro if y else. El codigo se veria mas o menos así:

 ```
 let hora = 23;

 if (hora>=0 &&hora<=5) {
  console.log("Dejame dormir");
 } else if (hora>=6 &&hora<=11) {
  console.log("Buenos días");
 } else if (hora>=12 &&hora<=18) {
  console.log("Buenas tardes");
 } else {
  console.log("Buenas noches");
 }



if (hora>0 &&hora<6) {
 console.log("Dejame dormir");
} else if (hora>5 &&hora<12) {
 console.log("Buenos días");
} else if (hora>11 &&hora<19) {
 console.log("Buenas tardes");
} else {
 console.log("Buenas noches");
}
 ```

 ### Operador ternario

 El operador ternario es como la simplificación de una estructura condicional tiene 3 partes: Consta de una condición (()), luego un signo de interrogación que significa la parte verdadera (?) y luego de dos puntos que consta de la parte falsa (:): Operador Ternario (condición) ? verdadero : falsa

### Switch case

El Switch case nos va a servir cuando nosotros tengamos diferentes valores en una misma variable.

La palabra brake dentro de nuestro switch, es lo que nos va a permitir que se salga del switch y no se pase de largo leyendo todos los casos (case)

El case, es el caso, es decir, lo que nosotros queremos que lea.

El default es cuando la variable en cuestion no cae en ninguno caso; así que, como su nombre lo indica, el valor va a caer en default por defecto.

En codigo se veria así:

```
switch (dia) {
  case 0:
    console.log("Domingo");
    break;
  case 1:
    console.log("Lunes");
    break;
    case 2:
    console.log("Martes");
    break;case 3:
    console.log("Miercoles");
    break;case 4:
    console.log("Jueves");
    break;case 5:
    console.log("Viernes");
    break;case 6:
    console.log("Sabado");
    break;
    
  default:
    console.log("Ese día no existe");
    break;
}
```

