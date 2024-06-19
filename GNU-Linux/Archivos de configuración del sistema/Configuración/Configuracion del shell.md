# Función
Los archivos de configuración del shell sirven para definir variables de entorno, [[Establecer Alias|establecer alias de comandos]], personalizar el comportamiento del shell y cargar scripts de inicio. Estas configuraciones determinan cómo se comporta el shell y cómo interactúa el usuario con el sistema.
# Ruta
En **Debian** se encuentra en -> `/etc/bashrc` o `/etc/zshrc`.
En esta ubicación se encuentran todas las shell disponibles en el sistema -> `/etc/shells`.
# Estructura
`variable_name=valor`
## Ejemplo:
```
PATH=/usr/local/bin:/usr/bin:/bin 
HOME=/home/usuario
```
# Notas:
- El nombre puede cambiar dependiendo del shell en uso del sistema.
- Bash se abre mediante `sudo nano ~/.bashrc`.
- Zsh se abre mediante `sudo nano ~/.zshrc`.
## Relacionados:
- [[Variables de entorno]]
- [[Alias de comandos]]
### [[Index_config|Volver al indice de Configuracion]]

#Shell #Configuracion