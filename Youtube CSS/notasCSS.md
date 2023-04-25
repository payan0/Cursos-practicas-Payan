# CSS

## Agrupación de elementos

Cuando queramos agregarle a ciertos elementos HTML mismos estilos, utilizamos la agrupación de elementos; la cual vamos utilizar un coma para eso (,)

Entonces, esto nos sirve para agrupar elementos HTML para darle ciertas reglas, esto solo usando la coma. 

Quedaría así:
```
.form-agrupar-selectores input[type="text"],
.form-agrupar-selectores input[type="email"],
.form-agrupar-selectores textarea {
    border-color: yellow;
    border-width: 2px;
    border-style: dashed;
    background-color: black;
    font-size: 20px;
    display: block;
    width: 300px;
}
```

---

## El algoritmo de CSS

El Algoritmo de CSS: Es la forma en el que el navegador aplica los estilos al documento HTML. Es vital entender este concepto para que entiendas como se aplican y en algunas ocasiones se sobreescriben las reglas.

El algoritmo de CSS se puede dividir en 3 partes:

**La cascada**: La cascada, va ser el mecanismo que tiene el navegador web para ir aplicando los estilos, y, en base a esto, toma 3 aspectos en particular:

*El origen del codigo*: Es de donde viene el codigo. Y por el origen del codigo, viene 3 posibles origenes: 

   *Usser agent*: No es más que los estilos que va aplicando el navegador por defecto a las etiquetas. Son los estilos por defecto del navegador

   La segunda opción seria todas las persolización que nosotros le hacemos al navegador o al sistema operativo.

   *Estilos del autor*: Eso ya son los estilos que nosotros les aplicamos en las hojas de CSS.


**La especificidad**: La especificidad es el peso que tiene un codigo de CSS. El codigo que tenga mayor peso, es el que se va a quedar, y es quien va a sobreescribir a los demas estilos.
Esto quiere decir que, a pesar de que un codigo este mas abajo que uno que este arriba, el codigo que tenga mas volumen es que va a ganar; sin importar la colocación.

Es por eso, que no necesitamos poner IDs, p

Cuando un estilo entra el conflicto con otro, entonces va a venir lo que va a diferenciar que estilo se aplica o no, eso va ser la especificidad. La especificidad, es lo que elige que estilo se va a aplciar o no, y el orden en que va apareciendo. 

La Especificidad es el peso que tiene un selector cuando hay conflictos de estilos. Se calcula de la siguiente forma:

Etiquetas y pseudoelementos -------------- 0,0,0,1

Clases, atributos y pseudoclases ------------ 0,0,1,0

Identificadores ----------------- 0,1,0,0

Estilos en línea ----------------- 1,0,0,0

!important ------------------- Rompe la especificidad


**La Herencia**: La Herencia, es la capacidad de un selector de obtener (heredar) los valores de sus ancestros más cercanos, para aplicarla se usa el valor inherit, si queremos evitarla podemos asignar otro valor o inicializar la propiedad en cuestión con el valor inicial

Algunos valores no se heredan: como el color de fondo, los bordes, entre otas. 

Las que si se heredan es todo lo que tenga que ver con la tipografia: el tamaño, la familia tipografica, etc.



---

## Propiedades

`border-color`: Sirve para dar color color al borde

`display`: Sirve para desplegar

`width`: Es para dar el ancho

`border-width`: Sirve para dar ancho al borde

`border-style`: Le da estilo al borde
