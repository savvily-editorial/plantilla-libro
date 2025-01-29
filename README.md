# Configuración

- Renombrar la carpeta **nombre-libro** con el nombre del nuevo libro.
- Los nombres de cada uno de los capítulos deberán estar enumerado y no deberán
  contener tildes ni caracteres especiales. Por ejemplo, el nombre del fichero para
  el capítulo 1 podría ser **01_nombre_capitulo.md**.
- Si existen subcapítulos, estos deberán estar contenidos en el capítulo
  principal y deberán seguir la misma estructura de enumeración, **en ningún caso
  un subcapitulo debe estar en un archivo diferente al del capitulo principal.**
  Se puede ver un ejemplo de como debería ser la estructura de los capitulos en los archivos de ejemplo.
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

# 📁 Estructura del libro

Este libro debera seguir el siguiente formato:

```
<nombre-del-libro-formato>
├── 01_capitulo.md
├── 02_capitulo.md
├── ...
├── 13_sabiduria.md
├── ...
├── resources
│   ├── portada-libro.png
│   ├── pub-data
│   ├── ...
├── templates
│   ├── opening.tex
│   ├── ...
└── Makefile
```

Dentro de la carpeta del libro unicamente deberemos tener los archivos que sean relativos a la generacion del libro, es decir, los capitulos, la portada, los recursos y los templates. Los capitulos deberan estar numerados de forma que se puedan ordenar de forma correcta, y deberan tener la extension `.md` o `.txt`. Los recursos deberan estar dentro de la carpeta `recursos` y los templates dentro de la carpeta `templates`.

## 🖥 Extensiones de VSCode

-   [Spell checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker):
    Checks mistakes in English and Spanish.
-   [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode):
    As our default formatter.
  -   Inside prettier config change `Prose wrap` value to `always`. This change
      should format Markdown as 80 characters max.
-   [Tabnine](https://www.tabnine.com/install/vscode): If you want some word
    completion.
-   [PDF visualizer](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf):
    Display pdf's in VSCode.