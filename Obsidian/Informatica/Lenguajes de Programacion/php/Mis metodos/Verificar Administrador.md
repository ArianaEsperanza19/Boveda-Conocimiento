Mediante la *session* 'admin' se verifica si el administrador tiene una sesión abierta. Si la sesión es existe y es igual a 1, entonces el admin esta activo.
```php
<?php

class verificarAdmin

{

public static function verificar()

{

$centinela = null;

if (isset($_SESSION['admin']) && $_SESSION['admin'] == true) {

$centinela = true;

}else{

$centinela = false;

}

return $centinela;

}

}
```

#### [[php-index-metodos|Volver a metodos]]