El `.` representa cualquier símbolo o carácter.

`l..e` -> Cualquier palabra que comience por *l*, termine en *e* y tenga dos elementos en medio. Ejemplo: `life

---
El `[]` representa un rango.

`[0-9]` -> Representa cualquier número entre 0 y 9.
`[a-z]` -> Representa cualquier letra en minúscula
`[A-Z]` -> Representar cualquier letra en mayúsculas.
Ejemplo: `t[eo]d` -> `today` o `tedious`

También puedes combinar rangos de caracteres de esta forma:

Cualquier letra en mayúsculas o minúsculas: `[a-zA-Z]`
Números del 1 al 5 y también del 9: `[1-59]`
Números del 1 al 5, letras de la a la f y también la X mayúscula:`[1-5a-fX]`
Ejemplo: `[a-zA-Z]` -> Cualquier palabra compuesta por letras.

---
El `^` representa negación o comienzo de un término.

`li [^ v] e` -> Todos los términos que comienzan con `li` y terminan con `e` pero no tienen ` i` o `v` en el interior. Ejemplo -> `like`
`^http` -> Un string que comienza con "http".

---
# Atajos
|**Operador**|**Descripción**|
|---|---|
|\w|Coincide con cualquier caracter de palabra (igual a `[a-zA-Z0-9_])`|
|\W|Coincide con cualquier otra cosa que no sea una letra, dígito o subrayado|
|\d|Coincide con cualquier dígito decimal. Equivalente a `[0-9]`|
|\D|Coincide con cualquier cosa que no sea un dígito decimal|

---
`()` representa agrupación como en matemáticas.

`(ab)*` -> Una o mas repeticiones de a y b en conjunto.
Ejemplo: `always`
`(ab)?` -> Lo mismo, pero buscara la repetición mas corta.

---
`*` 