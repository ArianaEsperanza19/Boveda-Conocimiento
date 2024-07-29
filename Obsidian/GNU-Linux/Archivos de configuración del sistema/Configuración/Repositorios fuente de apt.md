# Función
es un archivo de configuración crucial para el sistema de gestión de paquetes APT en distribuciones de Linux basadas en Debian, como Ubuntu, Mint y Debian. Este archivo define las fuentes de software que APT utiliza para buscar, descargar e instalar paquetes de software.
# Ruta
`/etc/apt/sources.list`
# Estructura
`deb/ [tipo] [url] [distribución] [componente]`
#### Descripción: 
`deb/`: Indica el tipo de archivo de paquete, en este caso "*deb*" para paquetes Debian.
`[tipo]`: Especifica el tipo de repositorio, como "*main*", "*stable*", "*testing*" o "*unstable*".
`[url]`: La URL del repositorio, que apunta a la ubicación del servidor que aloja los paquetes.
`[distribución]`: La distribución de Linux para la que se descargan los paquetes, como "*buster*", "*bullseye*" o "*jessie*".
`[componente]`: Los componentes específicos del repositorio, como "*main*", "*contrib*" o "*non-free*". Dichos componentes son:
- **Main**: Este componente contiene **software libre y de código abierto** que está **oficialmente mantenido por el equipo de Debian**. Estos paquetes cumplen con las directrices de software libre de Debian (DFSG) y son considerados esenciales para el funcionamiento del sistema o ampliamente utilizados por la comunidad.
- **Contrib**: Este componente contiene **software libre y de código abierto** que **no está oficialmente mantenido por el equipo de Debian**. Estos paquetes también cumplen con las DSFG, pero su mantenimiento recae en la comunidad o en desarrolladores externos.
- **Non-Free**: Este componente contiene **software propietario y de código cerrado** que **no cumple con las DSFG**. Estos paquetes requieren licencias adicionales o no están disponibles bajo licencias libres.
#### Ejemplo:
```
deb stable http://deb.debian.org/buster main contrib non-free
```
# Notas:
- Tras cualquier cambio es necesario actualizar la lista de paquetes mediante: `sudo apt update`
- Se recomienda comentar o eliminar las líneas de repositorios que no sean necesarios para evitar conflictos o errores durante la instalación de paquetes.
### [[Index_config|Volver al indice de Configuracion]]

#Configuracion #Repositorios 