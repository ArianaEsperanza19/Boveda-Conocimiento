# Nombre de procesos
- **ibus-daemon:** Este es el proceso principal de IBus que se encarga de iniciar y administrar el servicio IBus.
- **ibus-engine:** Este proceso se encarga de ejecutar el motor de entrada de método (IM) actual. El nombre exacto del proceso dependerá del motor de entrada de método que esté utilizando. Por ejemplo, si está utilizando el motor de entrada de método de Google Pinyin, el nombre del proceso sería `ibus-engine-pinyin`.
- **ibus-panel:** Este proceso es responsable de mostrar el panel de IBus en la barra de tareas.
- **ibus-daemon-bin:** Este es un binario auxiliar que se utiliza para iniciar el proceso `ibus-daemon`.
# Origen
Repositorios apt.
[https://github.com/ibus/ibus](https://github.com/ibus/ibus)
# Instalación
sudo apt install ibus ibus-m17n ibus m17n-db
sudo apt-get install ibus-anthy
# Función
IBus es un marco de entrada de método inteligente (IM) para sistemas operativos Linux. Permite a los usuarios cambiar fácilmente entre diferentes métodos de entrada de texto, como teclados fonéticos, teclados de símbolos y teclados de idiomas extranjeros. IBus también proporciona soporte para la entrada de escritura a mano y la entrada de voz.
## Comandos de [[Biblioteca de Comandos/Comandos/Comandos de apps y biblios/App/IBus|IBus]]
### Regresar a:
[[Index_app|Indice de Aplicaciones]]
[[Index_instaladas|Indice de Aplicaciones Instaladas]]

#Aplicaciones 