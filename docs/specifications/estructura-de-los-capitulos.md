# Estructura de los capítulos
- Los nombres de los archivos de cada uno de los capítulos deberá estar enumerado y no deberán contener tildes, caracteres especiales ni espacios en blanco. Por ejemplo, el nombre del fichero para el capítulo 1 debe ser `01_nombre_capitulo.md`. Este punto es muy importante para poder generar el libro de manera correcta.
- Si existen sub-capítulos, estos deberán estar contenidos en el capítulo principal, **en ningún caso un sub-capítulo debe estar en un archivo diferente al del capítulo principal.**
# Numeración de los capítulos
- Es muy importante numerar bien los capítulos ya que esta definición es la que va a generar el posterior índice del libro. Si los capítulos no están bien definidos no se generará correctamente el índice del libro.
### Capítulos
- Cada capítulo se marca con un título. El título se define con una sola `#`, el número del capítulo seguido de un punto y el nombre del capítulo, quedaría de esta manera `# 1. Capítulo`
### Sub-capítulos
- Los sub-capítulos y sub-sub-capítulos *nunca se enumeran*, solo los capítulos principales tienen numeración.
- Los sub-capítulo se define con dos `##`.
- Los sub-sub-capítulos se defienden con tres `###`.

```
# 1. Capítulo
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

## Sub-capítulo
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

### Sub-sub-capítulo
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

### Sub-sub-capítulo
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

## Sub-capítulo
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
```
- Al final de cada uno de los archivos de los capítulos es muy importante **dejar una línea en blanco**, esto es para que la generación del libro se realice de manera correcta. La herramienta que se utiliza para la generación del libro necesita que al final de cada archivo haya una línea en blanco para poder reconocer que el capítulo ha terminado y que el siguiente capítulo comienza.
### Resúmen de requisitos de la estructura de capítulos.
- Nombres de los archivos:
  - Enumerados con un formato de dos dígitos, 01, 02, 03, ... ✅
  - No deben contener tildes. ❌
  - No deben contener espacios ❌, en su lugar utilizaremos guiones medios `-`.✅
  - No deben contener caracteres especiales. ❌
- Capítulos:
  - Cada capítulo se marca con un título. El título se define con una sola `#`.
  - Contiene el número del capítulo seguido de un punto `2.`.
  - El resultado sería: `# 2. Name of chapter 2`.✅
  - Debe haber una línea en blanco al final de cada capítulo.👀
- Sub-capítulos:
  - Los sub-capítulos deben estar dentro de cada uno de los capítulos principales, en ningún caso estarán en archivos diferentes.
  - Los sub-capítulos y sub-sub-capítulos *nunca se enumeran*, solo los capítulos principales tienen numeración . El subtítulo se define con dos `##`.
    - `## Sub-capítulo`.✅
    - `### Sub-sub-capítulo`.✅

# 📁 Estructura de los ficheros del libro en el proyecto
Este libro deberá seguir el siguiente formato:

```
<nombre-del-libro-formato>
├── 01_capitulo.md
├── 02_capitulo.md
├── ...
├── 13_sabiduria.md
├── ...
├── resources
│   ├── front-cover.png
│   ├── pub-data
│   ├── ...
├── templates
│   ├── opening.tex
│   ├── ...
└── Makefile
```

Dentro de la carpeta del libro únicamente deberemos tener los archivos que sean relativos a la generación del libro, es decir, los capítulos, la portada, la contraportada, los recursos y los templates.

Los archivos de los capítulos deberán estar numerados de forma que se puedan ordenar de forma correcta, y deberán tener la extension `.md`.

Los recursos como son las imágenes, deberán estar dentro de la carpeta `recursos` y las plantillas dentro de la carpeta `templates`.
