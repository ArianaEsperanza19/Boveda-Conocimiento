```bash
#!/bin/bash
#Guardar salida de comando en una variable.

ubicacion=$(pwd)

echo $ubicacion

#Parametrizar variable.

nombre=$1

apellido=$2

#Deberan ser ingresadas en ese orden por la orden que ejecuta el fichero

echo "Hola, mi nombre es: $nombre $apellido"

#Para saber la cantidad de parametros recibidos

echo "La cantidad de parametros recibidos es $#"

#Para imprimir todos los paremetros enviados por el usuario

echo "Los parametros recibidos fueron $*"

#nota: Los parametros se pueden enviar entre comillas como por ejemplo "Ariana Esperanza"
```