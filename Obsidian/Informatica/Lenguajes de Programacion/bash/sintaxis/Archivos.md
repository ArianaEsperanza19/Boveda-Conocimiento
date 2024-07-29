# Manipulación de archivos mediante comandos
```bash
#!/bin/bash
input_type=''

input_name=''

input_extension=''

input_text=''

read -p "Desea generar un directorio(1) o un archivo(2): " input_type

#Crear un directorio

if(( $input_type == 1 ));then

read -p "Ingrese el nombre del directorio: " input_name

mkdir -m 777 $input_name

fi

#Crear un archivo

if(( $input_type == 2 ));then

read -p "Ingrese el nombre del archivo: " input_name

read -p "Ingrese la extension del archivo: " input_extension

archivo="${input_name}.${input_extension}"

read -p "Ingrese un texto para el archivo $archivo: " input_text

touch $archivo

echo $input_text >> $archivo

echo "Soy Ariana" >> $archivo

clear

cat $archivo

  

fi
```

# Leer archivo linea por linea
```bash
#!/bin/bash

input_name=$1

echo "===== Lectura de archivos ====="

echo "IFS (INTERNAL FIELD SEPARATOR), para leer linea por linea"
#Lee una linea completa y almacena el texto en $line
while IFS= read -r line || [[ -n "$line" ]]; do

echo "$line";

done < agenda.txt;
```

# Buscar y verificar archivo
```bash
#!/bin/bash
directorio="/ruta/a/tu/directorio"
archivo="mi_archivo.txt"

#El directorio es opcional, sin este parametro, se busca en el directorio actual.
if [ -e "$directorio/$archivo" ]; then
    echo "El archivo $archivo existe en $directorio."
else
    echo "El archivo $archivo no existe en $directorio."
fi

# Verificar si el archivo exite.
if [ -e "$archivo" ]; then

echo "El archivo $archivo existe."

fi
```