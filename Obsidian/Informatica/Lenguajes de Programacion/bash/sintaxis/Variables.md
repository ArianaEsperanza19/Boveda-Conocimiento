```bash
#!/bin/bash
# Variables
variable_de_Usuario="Soy una variable de usuario"

#Para especificar imprimir una variable es necesario anteponer el $

echo $variable_de_Usuario

#Imprimir una variable de entorno

echo "esta es una variable de entorno $PATH"

VARIABLE="Soy una variable de entorno creada por este script"
# Agrega una nueva variable de entorno a esta sesion, 
# por lo que al cerrar sesion, esta variable desaparecera.
export VARIABLE

echo $VARIABLE

#Nota importante: Las variables son sensibles a mayusculas o minusculas.
```