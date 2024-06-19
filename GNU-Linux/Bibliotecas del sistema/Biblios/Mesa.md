# Procesos
- **Mesa DRI:** Este proceso es responsable de la comunicación entre Mesa y el controlador del kernel de la tarjeta gráfica.
- **Mesa Xorg:** Este proceso proporciona la implementación de Xorg para Mesa, lo que permite que las aplicaciones X11 se comuniquen con Mesa.
- **Mesa GLX:** Este proceso proporciona la implementación de GLX para Mesa, lo que permite que las aplicaciones OpenGL se comuniquen con Mesa.
- **Mesa Vulkan:** Este proceso proporciona la implementación de Vulkan para Mesa, lo que permite que las aplicaciones Vulkan se comuniquen con Mesa.
# Origen
Repositorio kisak/mesa
https://www.mesa3d.org/
# Instalación
Si no lo tienes:
> sudo apt install mesa

Su ya lo tienes y quieres la ultima versión:
> sudo add-apt-repository ppa:kisak/mesa

> sudo apt install libglvnd-mesa-dev mesa-common-dev mesa-dev libvulkan-dev libglvnd-glx-dev

# Función
Es una biblioteca de software libre y de código abierto que ==juega un papel fundamental en el sistema gráfico de Linux==. Funciona como una capa de traducción entre las aplicaciones de gráficos y los controladores de la tarjeta gráfica, permitiendo que las aplicaciones se comuniquen con el hardware de manera eficiente.

## Comandos de [[Biblioteca de Comandos/Comandos/Comandos de apps y biblios/Biblio/Mesa|Mesa]]
### Regresar a:
[[Index_biblios|Indice de Bibliotecas]]
[[Indice maestro]]