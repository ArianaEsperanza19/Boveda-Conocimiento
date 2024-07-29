1. Crear un archivo .desktop con la siguiente estructura:
```
	[Desktop Entry]
	Type=Application
	Categories=Categoria
	Name=Nombre
	Icon=/ruta/al/icono
	Exec=/ruta/al/ejecutable
```
En el apartado de categorias debe ser uno de los siguientes tipos reconocibles:
**Categorías principales:**

Las categorías principales son amplias y agrupan aplicaciones por su función general. Algunos ejemplos de categorías principales incluyen:

- **Utility:** Aplicaciones de utilidad general, como editores de texto, calculadoras y visores de imágenes.
- **Game:** Juegos de ordenador.
- **Graphics:** Aplicaciones de gráficos, como editores de imágenes, visores de PDF y herramientas de diseño gráfico.
- **Office:** Aplicaciones de oficina, como procesadores de texto, hojas de cálculo y presentaciones.
- **Multimedia:** Aplicaciones multimedia, como reproductores de audio y vídeo, editores de vídeo y grabadoras de sonido.
- **System:** Aplicaciones de sistema, como herramientas de configuración, gestores de archivos y monitores de sistema.

**Subcategorías:**

Las subcategorías proporcionan una clasificación más específica dentro de las categorías principales. Por ejemplo, la categoría `Utility` puede tener subcategorías como `Calculator`, `Text Editor`, y `File Manager`.

**Categorías secundarias:**

Las categorías secundarias son opcionales y se pueden usar para proporcionar una clasificación aún más detallada. Por ejemplo, la categoría `Game` puede tener una categoría secundaria `Genre` con valores como `Action`, `Strategy`, y `Puzzle`.

**Selección de categorías:**

Al crear un ejecutable .desktop, es importante elegir las categorías adecuadas para su aplicación. Esto ayudará a los usuarios a encontrar su aplicación fácilmente en el menú de aplicaciones y otras interfaces gráficas.
2. Alojar dicho archivo en la ruta `/home/usuario/.local/share/applications`
3. Ejecutar en la terminal `sudo update-desktop-database`
### Regresar a:
[[Index_Enciclopedia|Indice de la enciclopedia]]
[[Indice maestro]]

---
#Enciclopedia #Utilidades #Tutorial
