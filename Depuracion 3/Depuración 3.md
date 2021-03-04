# Depuración 3

0. Importar el proyecto en vuestro WorkSpace de Eclipse.

1. Explicar QUÉ HACE EL MÉTODO MAIN.
Podéis poner líneas de código (prints) para ver cómo quedan las variables del programa, por ejemplo el vector.
    
    Se crean las variables:
    
    `int num;`
    
    `int c = 0, i = 0, enc = 0;`
    
    Crea el vector:
    
    `cosa [] lista = new cosa[kMAX];`
    
    Con un bucle while te pide que introduzcas 10 números que los almacena en num, asigna  `"enc=esta(lista,num);"` llamando al `"metodo esta"`, al introducir el número el bucle al ser `"enc mayor o igual que c"` introduce el primer número en la primera posicion del array, si introducimos el mismo número al ser `"enc menor que c"` añade un contador al número introducido, si introducimos un número distinto `"enc no sería menor que c"` añadiría el nuevo número a la siguiente posición del array.
    
    	public static void main(String[] args) {
    		// TODO Auto-generated method stub
    		
    		int num;
    		int c=0,i=0,enc=0;
    		Scanner sc = new Scanner(System.in);
    		
    		cosa [] lista = new cosa[kMAX];
		
		
    		while(i<kMAX) {
			
			System.out.println("Dime un numero: ");
			num=sc.nextInt();

			enc=esta(lista,num);
			if(enc<c) {
				lista[enc].setB(lista[enc].getB()+1);
			}
			else {
				lista[c] = new cosa(num);
				c++;
				
			}
		
			i++;
		}
    
    
2. Poner un punto de ruptura (breakpoint) en la línea 26 (primer bucle del método main) y, basándoos en los valores que van tomando las variables, explicad qué hace y cómo funciona el método. Podéis crear tablas para ver cómo cambian los valores de las variables y del array.

#### Valor incial de las variables:

![](Primera%20captura.png)

#### Al añadir el primer valor:

![](segunda%20captura.png)

> Como `enc` es igual o mayor que `c` introduce el número en la primera posición del array y le pone un contador de 1

#### Si ponemos el mismo valor

![](tercera%20captura.png)

> Ahora `c` e `i` valen 1 y se le añade un contador a la posición 0.

#### Si ponemos un valor distinto

![](Cuarta%20captura.png)

> `enc` valía 0 y `c` valía 1, por que lo que se añade el nuevo valor a la segunda posición del array con un contador de 1.

Si repitiesemos el proceso, siempre que repitamos un número nos sumaría 1 al contador de ese número y si ponemos uno nuevo añadiría el número al siguiente espacio del array hasta un máximo del 10 veces


3. Basándoos en el funcionamiento, determinad qué indican o a qué hacen referencia las variables “a” y “b” de la clase “cosa”.

“a” es el número que añadimospor teclado.

“b” es el contador de veces que ponemos el mismo valor.
