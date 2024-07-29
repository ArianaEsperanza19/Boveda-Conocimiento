Verificar los parámetros:
**host** = si se conectara al servidor local o a uno externo.
**dbname** = nombre de la base de datos para conectar.
**root** = nombre del usuario
**contraseña** = por ultimo, la contraseña, si esta es requerida.
```php
<?php

class DB{

public static function Connect(){

$conexion = new PDO("mysql:host=localhost;dbname=digitienda", "root", "");

$conexion->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);

//Asi se instanciaria mysqli.
//$conexion = new mysqli("localhost", "root", "", "digitienda");

#Para establecer el formato de escritura utf8.
$conexion->query("SET NAMES 'utf8'");

return $conexion;

}

}

?>
```

#### [[php-index-metodos|Volver a metodos]]