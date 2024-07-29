```bash
#!/bin/bash

#Declarar arreglo

#Los elementos se separan por espacios

numeros=(1 2 3 10)

nombres=(diego julian jennifer rosa miguel "Hernan Cortes")

rangos=({A..Z} {10..30})

echo "===== Imprimir valores ====="

echo "Arreglo numerico -> ${numeros[*]}" #Imprime todos los valores

echo "Arreglo de nombres -> ${nombres[*]}"

echo "Arreglo de rangos -> ${rangos[*]}"

echo "===== Imprimir tamaño de los arreglos ====="

echo ${#numeros[*]}

echo ${#nombres[*]}

echo ${#rangos[*]}

echo "===== Imprimir un elemento del arreglo ====="

echo "El segundo elemento del arreglo 'numeros': ${numeros[2]}"

echo "El segundo elemento del arreglo 'nombres': ${nombres[2]}"

echo "El segundo elemento del arreglo 'rangos': ${rangos[2]}"

echo "===== Manipular arreglo ====="

unset numeros[0] #Elimina un elemento

echo "Arreglo numerico sin el elemento # 0 -> ${numeros[*]}"

numeros[0]=1 # Agregar elemento en la posicion dada, el elemento que anteriormente ocupaba ese lugar sera empujado a la derecha

echo "Arreglo numerico devolviendo el elemento eliminado -> ${numeros[*]}"
```
# Ordenar arreglos
```bash
#!/bin/bash
#Ordenar arreglo

mi_arreglo=(5 2 10 1 8);

echo "===== Imprimir valores de arreglo ordenados ====="

# Ordenar el arreglo numerico de menor a mayor

sorted_arreglo=($(printf "%s\n" "${mi_arreglo[@]}" | sort -n))

echo ${sorted_arreglo[*]};

echo "================================================="

# Ordenar el arreglo numerico de mayor a menor (en reversa)

sorted_arreglo=($(printf "%s\n" "${mi_arreglo[@]}" | sort -nr))

echo ${sorted_arreglo[*]};
```