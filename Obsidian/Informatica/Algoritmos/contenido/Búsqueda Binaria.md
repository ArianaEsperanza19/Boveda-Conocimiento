El algoritmo de búsqueda binaria es un método eficiente para encontrar un elemento específico dentro de un conjunto de datos ordenado. Funciona dividiendo repetidamente la porción del conjunto de datos que podría contener el elemento buscado hasta reducir las ubicaciones posibles a solo una.

**Principio Básico:**

Imagine un libro de gran volumen con páginas numeradas. Si desea encontrar una palabra específica en el libro, no tendría que leer cada página una a una. En cambio, podría abrir el libro en el medio, ver la palabra de la página central y determinar si es la que busca.

- Si la palabra es la que busca, ¡la ha encontrado!
- Si la palabra es alfabéticamente anterior a la que busca, sabe que debe buscar en la primera mitad del libro.
- Si la palabra es alfabéticamente posterior a la que busca, sabe que debe buscar en la segunda mitad del libro.

Este proceso de dividir y descartar mitades se repite hasta que se encuentra la palabra o se determina que no está en el libro.

**Pasos del Algoritmo:**

1. **Definir el conjunto de datos ordenado:** El algoritmo de búsqueda binaria solo funciona con conjuntos de datos ordenados.
    
2. **Establecer el valor buscado:** El valor que se desea encontrar dentro del conjunto de datos ordenado.
    
3. **Inicializar índices:**
    
    - `inicio`: Variable que indica el índice del primer elemento del conjunto de datos.
    - `fin`: Variable que indica el índice del último elemento del conjunto de datos.
4. **Ciclo de búsqueda:**
    
    - Calcular el índice `medio`: `(inicio + fin) / 2`.
        
    - Obtener el valor del elemento en el índice `medio`.
        
    - Comparar el valor del elemento `medio` con el valor buscado:
        
        - Si son iguales, el valor buscado se encuentra en el índice `medio`. ¡Fin de la búsqueda!
        - Si el valor del elemento `medio` es menor que el valor buscado, actualizar el valor de `inicio` a `medio + 1`.
        - Si el valor del elemento `medio` es mayor que el valor buscado, actualizar el valor de `fin` a `medio - 1`.
5. **Repetir el ciclo de búsqueda** mientras `inicio` sea menor o igual a `fin`.
    
6. **Si el ciclo termina sin encontrar el elemento, el valor buscado no está en el conjunto de datos.**
    

**Ejemplo Práctico:**

Supongamos que tenemos un conjunto de datos ordenado de números enteros: {1, 3, 9, 15, 64, 97, 100}. Queremos encontrar el número 64.

**Pasos:**

1. **Conjunto de datos ordenado:** {1, 3, 9, 15, 64, 97, 100}
    
2. **Valor buscado:** 64
    
3. **Inicializar índices:**
    
    - `inicio = 0`
    - `fin = 6`
4. **Ciclo de búsqueda:**
    
    - `medio = (inicio + fin) / 2 = (0 + 6) / 2 = 3`
        
    - Valor en `medio`: {1, 3, 9, **15**, 64, 97, 100}
        
    - Comparar: 15 != 64
        
        - `inicio = medio + 1 = 4`
        - `fin = fin`
    - `medio = (inicio + fin) / 2 = (4 + 6) / 2 = 5`
        
    - Valor en `medio`: {1, 3, 9, 15, **64**, 97, 100}
        
    - Comparar: 64 = 64
        
        - ¡El valor buscado 64 se encuentra en el índice 5! Fin de la búsqueda.

**Ventajas del Algoritmo de Búsqueda Binaria:**

- **Eficiencia:** Es un algoritmo muy rápido, especialmente para conjuntos de datos grandes.
- **Escalabilidad:** Su eficiencia se mantiene incluso con conjuntos de datos de gran tamaño.
- **Simplicidad:** El concepto y la implementación son relativamente sencillos.

**Desventajas del Algoritmo de Búsqueda Binaria:**

- **Requiere datos ordenados:** Solo funciona con conjuntos de datos ordenados.
- **No es adecuado para inserciones o eliminaciones:** No está diseñado para insertar o eliminar elementos en el conjunto de datos.

**Conclusión:**

El algoritmo de búsqueda binaria es una herramienta poderosa y eficiente para encontrar elementos específicos dentro de conjuntos de datos ordenados. Su simplicidad, escalabilidad
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

# $inicio -le $fin

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