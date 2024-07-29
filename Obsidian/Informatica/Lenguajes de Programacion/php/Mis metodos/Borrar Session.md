Este método estático permite borrar la sesión recibida por parámetro.
```php
<?php

class borrarSession

{

public static function borrar($nombre)

{

if (isset($_SESSION[$nombre])) {

$_SESSION[$nombre] = null;

unset($_SESSION[$nombre]);

}

return $nombre;

}

}
```

#### [[php-index-metodos|Volver a metodos]]