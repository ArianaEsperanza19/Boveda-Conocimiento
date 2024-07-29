# Notación mnemónica

| Carácter | Permiso            |
| -------- | ------------------ |
| w        | Escritura          |
| x        | Ejecución y acceso |
| r        | Lectura            |
| -        | ninguno            |
**Orden de los permisos:** -rwx o drwx según sea un archivo o un directorio respectivamente. Son tres rwx (usuario, grupo y otros) y un guion (salvo el primero) por cada permiso no otorgado.
**Ejemplo:** 
`rw-r--`: Permisos de lectura y escritura para el propietario, permiso de lectura para el grupo y sin permisos para otros usuarios.
# Notación octal

| Dígito | Permiso | Descripción                    | Propietario | Grupo | Otros |
| ------ | ------- | ------------------------------ | ----------- | ----- | ----- |
| 0      | -       | Sin permiso                    | -           | -     | -     |
| 1      | x       | Ejecución                      | x           | -     | -     |
| 2      | w       | Escritura                      | -           | w     | -     |
| 3      | wx      | Escritura y ejecución          | x           | w     | -     |
| 4      | r       | Lectura                        | r           | -     | -     |
| 5      | rx      | Lectura y ejecución            | r           | x     | -     |
| 6      | rw      | Lectura y escritura            | r           | w     | -     |
| 7      | rwx     | Lectura, escritura y ejecución | r           | w     | x     |
**Orden de los permisos:**
- El primer dígito es para el propietario del archivo.
- El segundo dígito es para el grupo al que pertenece el archivo.
- El tercer dígito representa a otros usuarios.

| Permisos | Descripción                                                                                                                                  |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **777**  | Permisos completos para todos: propietario, grupo y otros usuarios. Lectura, escritura y ejecución para todos.                               |
| **755**  | Permisos completos para el propietario: lectura, escritura y ejecución. Lectura y ejecución para el grupo y otros usuarios.                  |
| **750**  | Permisos completos para el propietario: lectura, escritura y ejecución. Lectura y ejecución para el grupo. Sin permisos para otros usuarios. |
| **700**  | Permisos completos para el propietario: lectura, escritura y ejecución. Sin permisos para el grupo ni para otros usuarios.                   |
| **644**  | El propietario tiene permisos de lectura y escritura. El grupo tiene permiso de lectura. Otros usuarios tienen permiso de lectura.           |
| **640**  | El propietario tiene permisos de lectura y escritura. El grupo tiene permiso de lectura. Otros usuarios no tienen ningún permiso.            |
| **600**  | Permisos de lectura y escritura solo para el propietario.                                                                                    |

[[Dar permisos y privilegios|Como dar permisos y privilegios a un usuario]]
### Regresar a:
[[Index_Enciclopedia|Indice de la enciclopedia]]
[[Indice maestro]]

#Enciclopedia #Permisos