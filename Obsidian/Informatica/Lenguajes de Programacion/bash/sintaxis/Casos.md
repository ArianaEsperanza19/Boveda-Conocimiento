```bash
#!/bin/bash

opcion=''

read -p "Ingrese una opcion [A-B]: " opcion

case $opcion in

"A") echo "Ha ingresado la opcion A";;

"B") echo "Ha ingresado la opcion B";;

[C-Z]) echo "Valor fuera de rango";;

*) echo "Por favor solo caracteres dentro del rango [A-B]";;

esac
```