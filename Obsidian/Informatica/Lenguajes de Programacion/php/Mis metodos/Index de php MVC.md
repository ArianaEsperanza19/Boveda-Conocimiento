Recibe un parametro por la url para determinar a que controlador estás llamando y si dicho controlador existe. Luego usa el nombre del controlador recibido por url para formar el nombre de la clase del controlador que se quiere llamar.
La clase se instancia.
Luego comprueba si se recibe action por la url, asi como si dicho metodo existe, se llama.
Si no existe, se redirige a la pagina especificada.
```php
require_once 'autoload.php';

#Comprobar si se llama un controlador por la url
if(@$_GET){

if(isset($_GET['controller'])){

$nombre_controlador = $_GET['controller'].'Controller'; //Se concatena Controller para formar el nombre completo del controlador

}else{

//echo "La pagina que buscas no existe";

exit();

}

#Comprobar si la clase del controlador existe

if(class_exists($nombre_controlador)){

$controlador = new $nombre_controlador();

#Comprobar si el metodo llamado mediante 'action' en la url, existe en el controlador dado

if(isset($_GET['action']) && method_exists($controlador, $_GET['action'])){

$action = $_GET['action'];

$controlador->$action();

}else{

//echo "La pagina que buscas no existe";

}

}else{

//echo "La pagina que buscas no existe";

}

}else{
#Se redirige.
header("Location: ?controller=Productos&action=index");

}
```

#### [[php-index-metodos|Volver a metodos]]