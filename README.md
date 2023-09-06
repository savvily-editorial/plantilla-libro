# Configuración

- Renombrar la carpeta **nombre-libro** con el nombre del nuevo libro.
- Los nombres de cada uno de los capítulos deberán estar enumerado y no deberán
  contener tildes ni caracteres especiales. Por ejemplo, el nombre del fichero para
  el capítulo 1 podría ser **01_nombre_capitulo.md**.
- Las imágenes que se utilicen en cada uno de los capítulos deberán ir
  ubicadas en una carpeta **resources** que se encontrará dentro de la
  carpeta **nombre-libro**.
- Las imágenes deberán utilizar la extensión **png**.

# Problema con el uso de comillas invertidas

Evitar el uso de las comillas invertidas (`) para indicar una palabra o 
frase como código. El sistema de generación de libros no permite generar 
un libro en el que se utilice las comillas invertidas fuera de un bloque
de código.

Ejemplo de como no debería utilizarse:

texto `código` texto

Las comillas invertidas (`) se pueden utilizar para crear un bloque de
código que abarque varias líneas de código. Dentro de ese bloque de código 
si se podrá utilizar también las comillas invertidas.

Ejemplo:

```
  código
  
  texto `código` texto
```


# Estructura del libro

El libro debería seguir la siguiente estructura:

```
<nombre-libro>
├── 01_nombre_capitulo.md
├── 02_nombre_capitulo.md
├── ...
├── resources
│   ├── portada.png
│   ├── contraportada.png
│   ├── ...
├── 

```


