```php
class IMGmanager {
    private $url_img;

    public function __construct($url_img) {
        $this->url_img = $url_img;
    }

    public function borrarImagen($imagen) {
        // Verificar si la imagen existe en el directorio
        if (file_exists($this->url_img . $imagen)) {
            // Borrar la imagen
            if (unlink($this->url_img . $imagen)) {
                return "Imagen borrada exitosamente.";
            } else {
                return "Error al borrar la imagen.";
            }
        } else {
            return "La imagen no existe en el directorio.";
        }
    }

    public function uploadImage($image) {
        if ($image['name'] !== NULL && $image !== false) {
            $fecha = new DateTime();
            $imageName = $fecha->getTimestamp() . '_' . $image['name'];
            $imagenTemporal = $image['tmp_name'];
            move_uploaded_file($imagenTemporal, $this->url_img . $imageName);
            return $imageName;
        } else {
            return NULL;
        }
    }
}

// Ejemplo de uso
$imgManager = new IMGmanager("assets/img/");
$imagen = "nombre_de_la_imagen.jpg";

// Borrar imagen
$resultadoBorrar = $imgManager->borrarImagen($imagen);
echo $resultadoBorrar;

// Subir imagen
$image = $_FILES['imagen'];
$resultadoSubir = $imgManager->uploadImage($image);
echo $resultadoSubir;
```