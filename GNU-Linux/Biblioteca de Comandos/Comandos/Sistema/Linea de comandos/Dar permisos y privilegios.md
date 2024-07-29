# chmod +*privilegio* *archivo/directorio*
---
#### Ejemplo con letras: 
**Permisos totales sobre un *archivo* para el usuario y de ejecución para todos los demás**
`chmod -rwxr-x ruta/archivo.extension`
**Permisos totales sobre un *directorio* para el usuario y de ejecución para todos los demás**
`chmod drwxr-x ruta/carpeta`
**Otorgar un permiso**

|                             | Comando                 |
| --------------------------- | ----------------------- |
| Quitar permiso de ejecución | `chmod -x ruta/carpeta` |
| Dar permiso de ejecución    | `chmod +x ruta/carpeta` |
**Nota: De esta manera se otorga o revoca un permiso a todos: el dueño, su grupo y otros.**

---
#### Ejemplo con números:
**Todos los permisos para el usuario, su grupo y otros:**
`chmod 777 ruta/archivo.extension` 

---
##### Nota: A menudo es necesario ejecutar este comando con sudo.

[[Permisos y privilegios|Mas informacion sobre los permisos]]
### [[Index_sistema|Volver]]

#Permisos #Usuarios 