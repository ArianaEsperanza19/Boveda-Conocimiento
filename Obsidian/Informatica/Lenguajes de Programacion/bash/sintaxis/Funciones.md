# Función con entrada de datos por teclado
```bash
#!/bin/bash
parametros () {

echo "Hola, soy $1"

}

read -p "Ingrese su nombre: " nombre
parametros $dato
```
# Función con parámetros que retorna un valor
```bash
#!/bin/bash
nombre=''

retornar () {

nombre="Soy $1 $2"

}
retornar Ariana Uribe

echo $nombre
```