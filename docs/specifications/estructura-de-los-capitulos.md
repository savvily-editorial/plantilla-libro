# Estructura de los capítulos
- Los nombres de los archivos de cada uno de los capítulos deberá estar enumerado y no deberán contener tildes, caracteres especiales ni espacios en blanco. Por ejemplo, el nombre del fichero para el capítulo 1 debe ser `01_nombre_capitulo.md`. Este punto en muy importante para poder generar el libro de manera correcta.
- Si existen sub-capítulos, estos deberán estar contenidos en el capítulo principal y deberán seguir la misma estructura de enumeración, **en ningún caso un sub-capítulo debe estar en un archivo diferente al del capítulo principal.** Es muy importante numerar bien capítulos, sub-capítulos, etc., ya que esta definición es la que va a generar el posterior índice del libro. Si los capítulos y sub-capítulos no están bien definidos no se generará correctamente el índice del libro.  Por ejemplo de la siguiente manera.
```
# 2. Name of chapter 2
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

## 2.1. Section 1
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

### 2.1.1. Subsection 1
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

### 2.1.2. Subsection 2
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

#### 2.1.1.1. Subsubsection 1
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
```
- Al final de cada uno de los archivos de los capítulos es muy importante dejar una línea en blanco, esto es para que la 
generación del libro se realice de manera correcta. La herramienta que se utiliza para la generación del libro es `pandoc` 
y esta herramienta necesita que al final de cada archivo haya una línea en blanco para poder reconocer que el capítulo ha 
terminado y que el siguiente capítulo comienza.
### Resúmen de requisitos de la estructura de capítulos.
- Nombres de los archivos:
  - Enumerados con un formato de dos dígitos, 01, 02, 03, ...
  - No deben contener tíldes.
  - No deben contener espacios, en su lugar utilizaremos guiones medios `-`.
  - No deben contener caracteres especiales.
- Capítulos:
  - Cada capítulo se marca con un título. El título de define con una sola `#`.
  - Contiene el número del capítulo seguido de un punto `2.`.
  - El resultado sería: `# 2. Name of chapter 2`.
  - Debe haber una línea en blanco al final de cada capítulo.
- Sub-capítulos:
  - Los sub-capítulos deben estar dentro de cada uno de los capítulos principales, en ningún caso estarán en archivos diferentes.
  - Cada sub-capítulo se marca con un subtítulo. El subtítulo de defíne con dos `##`.
    - `## 2.1. Name of sub-chapter 2.1`.

# 📁 Estructura de los ficheros del libro en el proyecto
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

Dentro de la carpeta del libro únicamente deberemos tener los archivos que sean relativos a la generación del libro, es decir, los capítulos, la portada, los recursos y los templates.

Los capítulos deberán estar numerados de forma que se puedan ordenar de forma correcta, y deberán tener la extension `.md`.

Los recursos como son las imágenes, deberán estar dentro de la carpeta `recursos` y las plantillas dentro de la carpeta `templates`.
