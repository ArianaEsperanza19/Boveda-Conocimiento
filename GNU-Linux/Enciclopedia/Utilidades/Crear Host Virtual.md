# Configurar Host Virtual en Xampp en Linux
1. Ir al fichero *httpd-vhosts.conf* y modificar agregando lo siguiente:
```
<VirtualHost *:80>
       DocumentRoot "/opt/lampp/htdocs/"
       ServerName localhost
</VirtualHost>
```
Luego, para un nuevo anfitrion, escribe el nombre del dominio y la ruta:
```
<VirtualHost *:80>
    ServerName midominio.local
    DocumentRoot /ruta/a/tu/proyecto
</VirtualHost>
```
2. Ir al archivo ``/etc/hosts`` y agregar una entrada para el nuevo dominio.
```
127.0.0.1   midominio.local
```
3. Guardar cambios en los archivos y reiniciar Xampp.
4. Ingresar nuevo dominio en el navegador para acceder.