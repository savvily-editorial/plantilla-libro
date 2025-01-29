# Estructura de los capítulos
- Los nombres de cada uno de los capítulos deberá estar enumerado y no deberán contener tildes ni caracteres especiales. Por ejemplo, el nombre del fichero para el capítulo 1 debe ser `01_nombre_capitulo.md`.
- Si existen subcapítulos, estos deberán estar contenidos en el capítulo
  principal y deberán seguir la misma estructura de enumeración, **en ningún caso un subcapitulo debe estar en un archivo diferente al del capitulo principal.** Por ejemplo de la siguiente manera.
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

Dentro de la carpeta del libro unicamente deberemos tener los archivos que sean relativos a la generacion del libro, es decir, los capitulos, la portada, los recursos y los templates.

Los capitulos deberan estar numerados de forma que se puedan ordenar de forma correcta, y deberan tener la extension `.md`.

Los recursos deberan estar dentro de la carpeta `recursos` y las plantillas dentro de la carpeta `templates`.
