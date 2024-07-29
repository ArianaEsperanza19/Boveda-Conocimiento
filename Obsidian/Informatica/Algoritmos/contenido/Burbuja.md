El algoritmo de ordenación burbuja (Bubble Sort en inglés) es un algoritmo de ordenación simple y fácil de entender. Funciona recorriendo repetidamente una lista de elementos, comparando cada par de elementos adyacentes y, si es necesario, intercambiándolos de posición para que el elemento más pequeño quede antes que el más grande.

**Pasos del algoritmo:**

1. **Recorrer la lista:** Se inicia un bucle que recorre la lista desde el principio hasta el final.
    
2. **Comparar elementos adyacentes:** En cada iteración del bucle, se comparan dos elementos adyacentes de la lista.
    
3. **Intercambiar elementos:** Si el primer elemento es mayor que el segundo, se intercambian sus posiciones en la lista.
    
4. **Repetir:** El bucle se repite hasta que no se hayan realizado intercambios en la última iteración. Esto indica que la lista está ordenada.
    

**Ejemplo:**

Consideremos la lista desordenada [5, 2, 4, 1, 3]:

**Iteración 1:**

- Se comparan 5 y 2. Se intercambian porque 5 es mayor.
- La lista queda: [2, 5, 4, 1, 3]

**Iteración 2:**

- Se comparan 2 y 5. No se intercambian porque 2 es menor.
- Se comparan 5 y 4. Se intercambian porque 5 es mayor.
- La lista queda: [2, 4, 5, 1, 3]

**Iteración 3:**

- Se comparan 2 y 4. No se intercambian porque 2 es menor.
- Se comparan 4 y 5. No se intercambian porque 4 es menor.
- Se comparan 5 y 1. Se intercambian porque 5 es mayor.
- La lista queda: [2, 4, 1, 5, 3]

**Iteración 4:**

- Se comparan 2 y 4. No se intercambian porque 2 es menor.
- Se comparan 4 y 1. No se intercambian porque 4 es menor.
- Se comparan 1 y 5. No se intercambian porque 1 es menor.
- Se comparan 5 y 3. Se intercambian porque 5 es mayor.
- La lista queda: [2, 4, 1, 3, 5]

**Iteración 5:**

- Se comparan 2 y 4. No se intercambian porque 2 es menor.
- Se comparan 4 y 1. No se intercambian porque 4 es menor.
- Se comparan 1 y 3. No se intercambian porque 1 es menor.
- Se comparan 3 y 5. No se intercambian porque 3 es menor.
- Como no se realizaron intercambios, la lista está ordenada.

**Ventajas del algoritmo de ordenación burbuja:**

- **Simpleza:** Es uno de los algoritmos de ordenación más fáciles de entender e implementar.
- **Eficiencia en casos pequeños:** Para listas pequeñas, el algoritmo de ordenación burbuja puede ser eficiente.
- **In-place:** No requiere memoria adicional para almacenar datos temporales, ya que realiza la ordenación en la misma lista.

**Desventajas del algoritmo de ordenación burbuja:**

- **Ineficiencia en casos grandes:** Para listas grandes, el algoritmo de ordenación burbuja puede ser muy ineficiente, ya que realiza comparaciones y posibles intercambios cuadráticos (O(n^2)).
- **Peor caso:** El peor caso del algoritmo de ordenación burbuja es O(n^2), lo que significa que el tiempo de ejecución aumenta cuadráticamente con el tamaño de la lista.
- **Movimientos innecesarios:** El algoritmo puede realizar muchos intercambios innecesarios, incluso si la lista ya está casi ordenada.
# Ejemplo
```bash
#!/bin/bash

# 9. Implementa un algoritmo de búsqueda:
# Escribe un programa que implemente un algoritmo de búsqueda, como búsqueda binaria o búsqueda en anchura,
# para encontrar un elemento específico en una lista o matriz ordenada.

# Ordenar la lista
lista=(5 2 4 1 3);

longitud=${#lista[*]};

lista=($(printf "%s\n" "${lista[@]}" | sort -n))
# La lista ahora esta ordenada.

busqueda=2;

control=0;

mitad=$(($longitud/2));

pivote=$mitad;

inicio=0;

fin=$((longitud-1));

echo "busqueda: $busqueda";

# 1 2 3 4 5
while [ $control = 0 ]

do

if (( ${lista[$pivote]} == $busqueda )); then

control=1;

echo "Encontrado en la posicion $pivote";

break;

fi

if (( ${lista[$pivote]} > $busqueda )); then

pivote=$((pivote - 1));

fi

if (( ${lista[$pivote]} < $busqueda )); then

pivote=$((pivote + 1));

fi

if (( $pivote > $fin )) || (($pivote < $inicio )); then

echo "No encontrado";

break

fi

done
```