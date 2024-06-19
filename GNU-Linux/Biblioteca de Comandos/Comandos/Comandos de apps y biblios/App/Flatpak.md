### Tipo: Aplicación
### [[Biblioteca de Aplicaciones/Apps/Flatpak|Info]]
## Instalar una aplicación desde un repositorio
> flatpak install *nombre-aplicacion* [--remote *repositorio*]

**Ejemplo:** 
> flatpak install firefox flathub
## Busca una aplicación en los repositorios agregados
> flatpak search *nombre-aplicacion*
## Busca una aplicación en un repositorio específico
>flatpak search --remote *repositorio* *nombre-aplicacion*
## Muestra información sobre una aplicación instalada
> flatpak info *nombre-aplicacion*
## Muestra una lista de todas las aplicaciones instaladas
> flatpak list --app
## Listar todas las aplicaciones por su nombre
> flatpak list --app --columns=application
## Listar todas las aplicaciones y bibliotecas
> flatpak list
## Actualización
- `flatpak update`: Actualiza los repositorios agregados.
- `flatpak upgrade`: Actualiza las aplicaciones instaladas.
## Actualizar una aplicación
> flatpak update *application-name*

## Desinstala una aplicación
> flatpak uninstall *nombre-aplicacion*
## Agregar nuevo repositorio
> flatpak remote-add --if-not-exists *alias* *https://Repositorio_url*
## Lista los repositorios agregados
> flatpak remote-list
## Elimina un repositorio
> flatpak remote-delete *nombre*
## Limpiar paquetes huérfanos
>flatpak uninstall --unused
## Reparar aplicación
>flatpak repair *app-name*
## Ejecuta una aplicación con un comando especifico
> flatpak run *nombre-aplicacion* *comando*
---
### Regresar a:
[[Index_apps_biblios|Indice de apps y biblios]]
[[Index_comandos|Indice de comandos]]
[[Indice maestro]]

#Paqueteria #Comandos #Aplicaciones #Non-Grafica 

