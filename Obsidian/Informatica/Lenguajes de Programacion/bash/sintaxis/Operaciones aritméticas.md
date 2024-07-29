```bash
#!/bin/bash

numA=4

numB=2

# Esta es la sintaxis para hacer operaciones matematicas

echo $((numA+numB)) # Suma

echo $((numA-numB)) # Resta

echo $((numA*numB)) # Multiplicacion

echo $((numA/numB)) # Division

echo $((numA%numB)) # Residuo

echo $((numA**numB)) # Potencia

echo "scale=4; sqrt($numA)" | bc # Raiz cuadrada

echo "scale=0; $raiz/1" | bc -l; # Redondeo

```