```php
<?php

function autocargar($classname){

include 'controllers/' . $classname . '.php';

}
spl_autoload_register('autocargar');
```

#### [[php-index-metodos|Volver a metodos]]
