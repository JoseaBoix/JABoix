# Depuración 2

**Importar el proyecto en vuestro WorkSpace de Eclipse.**

**Explicar QUÉ HACE EL MÉTODO MAIN.**
    
1.      Crea e inicializa la variable kMAX y crea 2 array llamados lista y lista2 con tamaño de kMAX.
2.      Utiliza el método rellenarArrays en lista y  en lista2.
3.      Imprime los números utilizando el método imprimnirArray(lista); en el orden de creación. 
4.      Utiliza el método intercambio(lista); para ordenar los números generados de menor  a mayor.
5.      Los imprime utilizando el método imprimnirArray(lista);.
6.      Repite  el proceso desde el punto 3 pero con lista2, pero utilizando el método countingSort(); para ordenar lista2.

     
**Poner un punto de ruptura (breakpoint) en la línea 78 (primer bucle del método intercambio) y, basándoos en los valores que van tomando las variables, explicad cómo funciona el método de ordenación de arrays por intercambio. Podéis crear tablas para ver cómo cambian los valores de los arrays.**

<table>
<thead>
	<tr>
	    <th>Lista inicial</th>
		<td>83,67,69,16,96,61,56,89,47,57</td>
	</tr>
</thead>
<tbody>
	<tr>
	    <th>Lista bucle 1</th>
		<td>67,83,69,16,96,61,56,89,47,57</td>
	</tr>
		<tr>
	    <th>Lista bucle 2</th>
		<td>16,83,69,67,96,61,56,89,47,57</td>
	</tr>
		<tr>
	    <th>Lista bucle 3</th>
		<td>16,69,83,67,96,61,56,89,47,57</td>
	</tr>
		<tr>
	    <th>Lista bucle 4</th>
		<td>16,67,83,69,96,61,56,89,47,57</td>
	</tr>
			<tr>
	    <th>Lista bucle 5</th>
		<td>16,61,83,69,96,67,56,89,47,57</td>
	</tr>
</tbody>
</table>
El primer bucle selecciona la primera posición, el segundo bucle recorre el array buscando el número menor y lo inserta en la primera posición y el que ocupaba esta posición lo inserta en la queocupaba el número menor, el primer bucle selecciona la segunda posición y busca el siguiente número menor del array e intercambia posiciones con el número que ocupaba la segunda posición. y así hasta que ordena todo el array.

**Poner un punto de ruptura (breakpoint) en la línea 94 y explicad cómo funciona el método de ordenación de arrays de conteo. Podéis crear tablas para ver cómo cambian los valores de los arrays.
Nota: Realizad las capturas de pantalla que creáis conveniente para adjuntar en el documento.
(por ejemplo los valores de la ventana de VARIABLES de la perspectiva DEBUG)**

<table>
<thead>
	<tr>
	    <th>numero generado 1</th>
		<td>19</td>
	</tr>
</thead>
<tbody>
	<tr>
	    <th>número generado 2</th>
		<td>94</td>
	</tr>
		<tr>
	    <th>número generado 3</th>
		<td>45</td>
	</tr>
		<tr>
	    <th>número generado 4</th>
		<td>72</td>
	</tr>
		<tr>
	    <th>número generado 5</th>
		<td>98</td>
	</tr>
		<tr>
	    <th>número generado 6</th>
		<td>74</td>
	</tr>
		<tr>
	    <th>número generado 7</th>
		<td>36</td>
	</tr>
		<tr>
	    <th>número generado 8</th>
		<td>87</td>
	</tr>
		<tr>
	    <th>número generado 9</th>
		<td>70</td>
	</tr>
		<tr>
	    <th>número generado 10</th>
		<td>42</td>
	</tr>
</tbody>
</table>

Este bucle  recorre del 1 al 100 y cuando encuentra un número de la lista suma un contador, despues ordena los números encontrados según la posición del contador.