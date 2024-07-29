*Parametro necesario*
~~Tipo de busqueda~~
==Elemento buscado==

---
# find *directorio_de_busqueda/* ~~tipo~~ *filtro_de_busqueda* ==Fichero.extension==
---
## Parámetros de búsqueda
### Buscar por nombre `-name`
### Tipos de archivos
- `-type d` Busca directorios.
- `-type f` Busca archivos regulares (archivos que contienen datos, como documentos de texto, imágenes, etc.).
- `-type l` Busca enlaces simbólicos (enlaces a otros archivos o directorios).
- `-type s`  Busca sockets (archivos especiales para la comunicación entre procesos).
- `-type p`  Busca pipes (archivos especiales para la transferencia de datos entre procesos).
- `-type b`  Busca dispositivos de bloque (archivos que almacenan datos en bloques, como discos duros).
- `-type c` Busca dispositivos de caracter (archivos que se acceden de uno en uno, como teclados y puertos serie).
### Atributos del archivo
- `-size +N`: Busca archivos que sean más grandes que N bytes.
- `-size -N`: Busca archivos que sean más pequeños que N bytes.
- `-mtime +N`: Busca archivos que se hayan modificado hace N días o más.
- `-mtime -N`: Busca archivos que se hayan modificado hace menos de N días.
- `-atime +N`: Busca archivos que se hayan accedido hace N días o más.
- `-atime -N`: Busca archivos que se hayan accedido hace menos de N días.
- `-perm NNN`: Busca archivos con permisos específicos. Los permisos se especifican como un número octal de 3 dígitos, donde cada dígito representa los [[Permisos y privilegios|permisos]] para el propietario, el grupo y otros usuarios.
### Nota:
`Si no devuelve nada, es posible que quieras verificar si el directorio esta correctamente escrito. La dirección debe terminar con un /`
### Regresar a: 
[[Index_archivos| Indice de comandos de archivos]]

#Comandos 