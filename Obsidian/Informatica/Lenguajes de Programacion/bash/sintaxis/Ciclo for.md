```bash
#!/bin/bash

#Declarar arreglo

#Los elementos se separan por espacios

numeros=(1 2 3 10)

nombres=(diego julian jennifer rosa miguel "Hernan Cortes")

rangos=({A..Z} {10..30})

echo "===== Iteracion de numeros ====="

#Foreach

for num in ${numeros[*]}

do

echo "Numero: $num"

done

echo "===== Iteracion de nombres ====="

#For tradicional

for((i=0;i<${#nombres[*]};i++))

do

echo "El nombre es: ${nombres[$i]}"

done
```