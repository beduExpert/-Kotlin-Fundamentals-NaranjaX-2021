## Condicionales 

### OBJETIVO 

- Poner en práctica ejemplos de condicionales

#### REQUISITOS 

1. Saber la sintaxis de la expresión *When*
2. Haber utilizado previamente la expresión *if*

#### DESARROLLO

1. Crear una función que pida como parámetros las medidas de los lados de un triángulo. Debe imprimirnos el tipo de tríangulo:

* Equilatero: los tres lados tienen el mismo valor
* Isóceles: Tiene dos lados iguales
* Escaleno: Los tres lados son diferentes

Utilizar la expresión condicional *if - else if - else* . Para evaluar más de un valor en la sentencia if, debemos utilizar los operadores lógicos ***&&*** (AND), ***||*** (OR) y ***!*** (NOT)

No olvides ejecutar varias pruebas para comprobar que tu algoritmo funciona correctamente!

<details>
	<summary>Solución</summary>
	
```kotlin
fun tipoDeTriangulo(lado1: Int, lado2: Int, lado3: Int){

    if(lado1==lado2 && lado2==lado3){
        println("Es un triángulo equilátero")
    } else if(
        (lado1==lado2 && lado3!=lado1 ) ||
        (lado2==lado3 && lado1!=lado2 ) ||
        (lado3==lado1 && lado2!=lado3) ){
        println("Es un triángulo isóceles")
    } else{
        println("Es un triángulo escaleno")
    }
}
```

</details>

2. Utilizando ***When*** define una función que recibe un número entero y te regresa el mes que representa, por ejemplo:

```kotlin
mes(5) = "mayo"
```

recuerda tratar con el caso de los número que no representan meses



[`Atrás`](../Ejemplo-02) | [`Siguiente`](../Ejemplo-03)


