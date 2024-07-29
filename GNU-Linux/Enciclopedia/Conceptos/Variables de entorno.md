Las variables de entorno almacenan información global sobre el sistema y el entorno del usuario, como la ruta de acceso a los directorios binarios, la configuración regional y el nombre de usuario. Los archivos de configuración del shell pueden definir o modificar estas variables para personalizar el entorno del usuario.
## Algunas variables de entorno son:
**1. PATH:**

- **Función:** Define la ruta de búsqueda que utiliza la shell para encontrar comandos ejecutables.
- **Ejemplo:** Si escribes `ls` en la terminal, la shell buscará el ejecutable `ls` en los directorios especificados en la variable `PATH`.

**2. HOME:**

- **Función:** Almacena la ruta del directorio personal del usuario actual.
- **Ejemplo:** Si escribes `cd ~/Documentos`, te moverás al directorio `Documentos` dentro de tu directorio personal.

**3. USER:**

- **Función:** Almacena el nombre de usuario del usuario actual.
- **Ejemplo:** El comando `whoami` imprime el valor de la variable `USER`.

**4. LANG:**

- **Función:** Define el idioma y la configuración regional del usuario.
- **Ejemplo:** La variable `LANG` puede establecerse en `es_ES.UTF-8` para usar español con codificación UTF-8.

**5. LC_CTYPE:**

- **Función:** Define la configuración regional del idioma para la entrada y salida de texto.
- **Ejemplo:** La variable `LC_CTYPE` puede establecerse en `es_ES.UTF-8` para usar el alfabeto español con codificación UTF-8.

**6. LC_MESSAGES:**

- **Función:** Define la configuración regional del idioma para los mensajes del sistema y las aplicaciones.
- **Ejemplo:** La variable `LC_MESSAGES` puede establecerse en `es_ES.UTF-8` para mostrar mensajes en español.

**7. LC_TIME:**

- **Función:** Define la configuración regional del idioma para el formato de fecha y hora.
- **Ejemplo:** La variable `LC_TIME` puede establecerse en `es_ES.UTF-8` para mostrar las fechas y horas en formato español.

**8. DISPLAY:**

- **Función:** Especifica la pantalla X11 a la que se deben enviar las aplicaciones gráficas.
- **Ejemplo:** La variable `DISPLAY` se establece automáticamente en la mayoría de los entornos de escritorio.

**9. HOSTNAME:**

- **Función:** Almacena el nombre de host del sistema.
- **Ejemplo:** El comando `hostname` imprime el valor de la variable `HOSTNAME`.

**10. TMPDIR:**

- **Función:** Define el directorio temporal que se utiliza para almacenar archivos temporales.
- **Ejemplo:** Las aplicaciones pueden usar la variable `TMPDIR` para crear archivos temporales en una ubicación específica.

**11. PS1:**

- **Función:** Define el símbolo del sistema, que es el texto que se muestra antes de cada línea de comando en la terminal.
- **Ejemplo:** Puedes personalizar el símbolo del sistema usando variables especiales como `\u` (nombre de usuario) y `\h` (nombre de host).

**12. HISTSIZE:**

- **Función:** Define el número máximo de entradas que se almacenan en el historial de comandos de la shell.
- **Ejemplo:** Un valor más alto de `HISTSIZE` te permite acceder a más comandos anteriores.

**13. EDITOR:**

- **Función:** Define el editor de texto predeterminado que se utiliza cuando se abre un archivo de texto desde la línea de comandos.
- **Ejemplo:** Puedes establecer `EDITOR` en `nano` o `vim` para usar tu editor de texto preferido.
### Regresar a:
[[Index_Enciclopedia|Indice de la enciclopedia]]
[[Indice maestro]]

---
#Enciclopedia #Variables_Entorno