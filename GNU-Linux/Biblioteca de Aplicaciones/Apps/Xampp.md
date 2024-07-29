# Nombre del proceso

# Origen

https://www.apachefriends.org/es/index.html
# Instalación
1. Descargar e instalar el paquete de Xampp junto con todos los core files.
2. Conceder permisos pertinentes a la carpeta /opt/lampp y las carpetas de los proyectos.
3. Configurar puertos 8889 y 3306 para la base de datos. Verificar puertos en uso mediante el comando `sudo lsof -i -P -n | grep LISTEN`.
4. Conectar a la base de datos mediante el puerto 8889.
# Función

**XAMPP** es una distribución gratuita y fácil de instalar que contiene **Apache**, **MariaDB**, **PHP** y **Perl**. Su función principal es proporcionar un entorno de desarrollo local para crear y probar aplicaciones web.
# Notas

- Modificar el archivo etc/profile para tener php en todos los directorios. Se debe agregar la siguiente linea `export PATH="$PATH:/opt/lampp/bin"` al final del documento.
- Verificar archivos de registros (logs) para encontrar errores, pues estos no aparecen en el navegador.
- Archivos de configuracion: my.cnf
- Para instalar Composer: https://getcomposer.org/download/
- Para instalar Laravel usando Composer: https://laravel.com/docs/11.x/installation
## Comandos de [[Biblioteca de Comandos/Comandos/Comandos de apps y biblios/App/Xampp|Xampp]]
## [[Crear Host Virtual]] para Xampp en Linux.
### Regresar a:

[Indice de Aplicaciones](app://obsidian.md/Index_app)  
[Indice de Aplicaciones Instaladas](app://obsidian.md/Index_instaladas)

[#Aplicaciones](app://obsidian.md/index.html#Aplicaciones)