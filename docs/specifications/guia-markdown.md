# Formato de texto del documento MarkDown

- **Texto en negrita**
    ```
    **Texto que deseamos que esté en negrita**
    ```
    **`Negrita`**
- **Texto en cursiva**
    ```
    *Texto que deseamos que esté en cursiva*
    ```
    *`Cursiva`*
- **Título:**
  ```
  # Titulo
  ```
  # `Título`
- **Subtítulo:**
  ```
  ## Subtitulo
  ```
  ## `Subtítulo`
- **Subtítulo secundario:**
  ```
  ### Subtitulo secundario
  ```
  ### `Subtítulo secundario`
- **Subtítulo terciario:**
  ```
  #### Subtitulo terciario
  ```
  #### `Subtítulo terciario`
- **Lista numerada:**
    ```
    1.
    2.
    3.
    ...
    ```
- **Lista sin numerar:**
    ```
    -
    -
    -
    ...
    ```
    
# Formato de texto del documento con LaTeX
- **Texto en negrita**
    ```
    \textbf{Texto que deseamos que esté en negrita}
    ```
    **`Negrita`**
- **Texto en cursiva**
    ```
    \textit{Texto que deseamos que esté en cursiva}
    ```
    *`Cursiva`*
- **Texto en cursiva**
    ```
    \emph{Texto que deseamos enfatizar}
    ```
    *`Cursiva`*
- **Texto subrayado**
    ```
    \underline{Texto que deseamos que esté subrayado}
    ```
- **Centrar texto**
    ```
    \begin{center}
    Texto que desees centrar
    \end{center}
    ```
- **Añadir imágen**
    ```
    \begin{figure}[H]
    \includegraphics[width=6cm]{./resources/figuras_geometricas.png}
    \end{figure}
    ```
    - **`\begin`**: Marca el inicio desde donde va a partir la imágen.
    - **`{figure}`** : Indica que vas a añadir una figura al documento.
    - **`[H]`**: Ancla la figura en el lugar donde se encuentra el código LaTeX, y no permite que LaTeX la mueva automáticamente a una página posterior o a otro lugar para mejorar el diseño.
    - **`\includegraphics`**: Indica que vamos a añadir una imágen.
        - **`[width=6cm]`**: Defíne el ancho de la imágen.
        - **`{./resources/figuras_geometricas.png}`**: Indica la ruta de la imágen.

- **Añadir imágen centrada**
    ```
    \begin{figure}[H]
    \centering
    \includegraphics[width=6cm]{./resources/figuras_geometricas.png}
    \end{figure}
    ```
    - **`\cenetring`**: Centra la imágen en la página.
- **Crear una tabla**
    ```
    \begin{tabular}{|c|c|c|}
    \hline
    Encabezado 1 & Encabezado 2 & Encabezado 3 \\
    \hline
    Celda 1,1 & Celda 1,2 & Celda 1,3 \\
    \hline
    Celda 2,1 & Celda 2,2 & Celda 2,3 \\
    \hline
    \end{tabular}

    ```
    ![](https://hackmd.io/_uploads/rkkm6F6gT.png)
- **Centrar la tabla**
    ```
    \begin{center}
    \begin{tabular}{|c|c|c|c|c|c|c|}
    \hline
    3x3 & 3x4 & 3x5 & 3x6 & 3x7 & 3x8 & 3x9\\\hline
    & 4x3 & 5x3 & 6x3 & 7x3 & 8x3 & 9x3\\\hline
    \end{tabular}
    \end{center}
    ```
    ![](https://hackmd.io/_uploads/ByOGIqalp.png)
    - **`\begin{center}`**: Centra la tabla en la página.
    - **`\begin{tabular}`**: Crea la tabla.
    - **`{|c|c|c|c|c|c|c|}`**: Define las columnas de la tabla.
    - **`\hline`**: lineas de la tabla.
    - **`\end{tabular}`**: Finaliza la tabla.
    - **`\end{center}`**: Finaliza el centrado.
- **Pie de pagina**
    ```
    \footnote[1]{Nota que deseas mostrar al pie de página}:
    ```
    `1. Nota que deseas mostrar al pie de página`
    
    
# Extras
## Herramientas para tranformar un documento a formato Markdown 🛠️

- [ChatGPT](https://chat.openai.com) - IA que te ayuda a resolver dudas y problemas de forma sencilla. Pidele que transforme tu texto a Markdown y lo hará. 🤖
- [Apose](https://products.aspose.app/words/es/conversion/doc-to-md) - Web para transformar archivos Word con extensión .doc a formato Markdown con extensión .md. 📄🔄
