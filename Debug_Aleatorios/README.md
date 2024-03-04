Al poner un breakpoint en el bucle y revisar los datos observamos que el problema está
en la asignación de los valores a las posiciones del array.
La función Math.random()devuelve un número decimal entre 0 y 1.
Al transformarlo a int vale 0. Entonces la operación estaba siendo => 0 * 100 = 0.
Para solucionar esto nos aseguramos que la multiplicación se ejecuta antes de transformar
el resultado a Integer
