Este método estático permite escapar los datos recibidos por parámetro, mediante mysqli.
```php
<?php

class escaparDatos

{

public static function escapar($datos){

//Escapa la informacion recibida para evitar fallos.

$mysqli = new mysqli("localhost", "root", "", "dataBase");

$mysqli->query("SET NAMES 'utf8'");

$datos = $mysqli->real_escape_string($datos);

$mysqli->close();

return $datos;

}

}

?>
```

#### [[php-index-metodos|Volver a metodos]]