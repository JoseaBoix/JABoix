# Depuración 1
1. En la función1… ¿Qué hacen estas líneas de código?

> String string2 = "string2";
> string2= string2.substring(0, string2.length()-1);

Esta linea de código resta 1 a la posición del String y elimina el 2, quedando string2 = string.

> string2=string2+"1";

Esta linea añade un 1 al string resultando string2 = string1.

2. ¿Qué valen las variables string1 y string2 antes de ejecutar el código de comprobación
siguiente?

> if(string1 == string2 ) {
> System.out.println("SON IGUALES " + a);
> }
> else {
> System.out.println("SON DIFERENTES");
> }

Tanto string1 como string2 valen string1.

3. ¿Por qué no funciona el operador == ? ¿Qué operador se debe usar en lugar de este?

Por que == compara los objetos instanciados y no el valor de la cadena
He usado .equals() quedando de la siguiente manera if(string1.equals(string2)).

4. La función2() está declarada como sigue:

> public void funcion2() {
> System.out.println("--------------------");
> System.out.println("Esta es la función 2");
> System.out.println("Cómo hago la llamada para que
> funcione????");
> }

He llamado a la funcion añadiendo funcion2(); y static a la función.
