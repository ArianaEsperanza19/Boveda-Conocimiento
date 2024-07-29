```bash
#!/bin/bash

name=''

age=''

#Para pedir datos al usuario

read -p "Ingresa tu nombre: " name

read -p "Ingresa tu edad: " age

#Verifica una condicion

if(( $age >= 18));then

echo "Soy mayor de edad"

else

echo "Soy menor de edad"

fi

echo "======================================================="

#Mas de una condicion

#Y &&

if [ $age -gt 18 ] && [ $name = 'Ariana' ]; then

# Se cumple la condición, ejecuta el código aquí

echo "La edad es mayor a 18 y el nombre es Ariana"

else

# La condición no se cumple, ejecuta el código aquí

echo "La edad no es mayor a 18 o el nombre no es Ariana"

fi

echo "======================================================="

#O ||

if [ $age -lt 18 ] || [ $age -gt 90 ]; then

# Se cumple la condición, ejecuta el código aquí

echo "No estas en condicion de sufragar"

else

# La condición no se cumple, ejecuta el código aquí

echo "Puedes sufragar"

fi
```
## Formato de las condiciones de bash

| Condición | Descripción       | Ejemplo                                                                                                |
| --------- | ----------------- | ------------------------------------------------------------------------------------------------------ |
| `-gt`     | Mayor que         | `if [ $edad -gt 18 ]; then echo "La edad es mayor a 18"; fi`                                           |
| `-lt`     | Menor que         | `if [ $edad -lt 18 ]; then echo "La edad es menor a 18"; fi`                                           |
| `-ge`     | Mayor o igual que | `if [ $edad -ge 25 ]; then echo "La edad es mayor o igual a 25"; fi`                                   |
| `-le`     | Menor o igual que | `if [ $edad -le 16 ]; then echo "La edad es menor o igual a 16"; fi`                                   |
| `-eq`     | Igual que         | `if [ $nombre = "Juan" ]; then echo "El nombre es Juan"; fi`                                           |
| `-ne`     | Distinto que      | `if [ $pais != "Venezuela" ]; then echo "El país no es Venezuela"; fi`                                 |
| `-and`    | Y                 | `if [ $edad -gt 18 ] && [ $sexo = "masculino" ]; then echo "Es mayor de edad y de sexo masculino"; fi` |
| `-or`     | O                 | `if [ $calificacion -ge 90 ]`                                                                          |
## Otros operadores condicionales
|Operador|Descripción|Ejemplo|
|---|---|---|
|`-f`|Verifica si un archivo existe y es un archivo normal|`if [ -f "archivo.txt" ]; then echo "archivo.txt es un archivo normal"; fi`|
|`-d`|Verifica si un archivo existe y es un directorio|`if [ -d "directorio" ]; then echo "directorio es un directorio"; fi`|
|`-s`|Verifica si un archivo existe y tiene un tamaño mayor que 0 bytes|`if [ -s "archivo.txt" ]; then echo "archivo.txt no está vacío"; fi`|
|`-x`|Verifica si un archivo existe y tiene permisos de ejecución para el usuario actual|`if [ -x "script.sh" ]; then echo "script.sh es ejecutable"; fi`|
|`-r`|Verifica si un archivo existe y tiene permisos de lectura para el usuario actual|`if [ -r "archivo.txt" ]; then echo "archivo.txt es legible"; fi`|
|`-w`|Verifica si un archivo existe y tiene permisos de escritura para el usuario actual|`if [ -w "archivo.txt" ]; then echo "archivo.txt es escribible"; fi`|
|`-e`|Verifica si una variable está definida y no está vacía|`if [ -e $variable ]; then echo "La variable $variable está definida y no está vacía"; fi`|
|`-n`|Verifica si una cadena no está vacía|`if [ -n "$cadena" ]; then echo "La cadena $cadena no está vacía"; fi`|
|`-z`|Verifica si una cadena está vacía|`if [ -z "$cadena" ]; then echo "La cadena $cadena está vacía"; fi`|