# LaTeX
# 📘 LaTeX

LaTeX es una herramienta para la composición de documentos de aspecto profesional que funciona mediante comandos de texto plano, permitiéndote enfocarte en el contenido mientras el sistema se encarga de la apariencia visual.

---

# 📦 Definición de la Clase del Documento

Todo documento de LaTeX debe comenzar declarando su clase, la cual controla el diseño general.

Para documentos estándar, se utiliza la clase `article`.

```latex
\documentclass{article}
```

---

# ⚙️ El Preámbulo y la Configuración del Título

El preámbulo es la sección de configuración que aparece antes del inicio del cuerpo del documento.

Aquí se define la información que aparecerá en el título:

- `\title{...}` → Título del documento.
- `\author{...}` → Nombre del autor.
- `\date{...}` → Fecha manual o `\today` para usar la fecha actual.

```latex
\title{Mi Documento}
\author{Juan Pérez}
\date{\today}
```

---

# 📄 Cuerpo del Documento

El contenido visible se escribe dentro del entorno delimitado por:

```latex
\begin{document}
...
\end{document}
```

Para que el título aparezca en el PDF, debes usar:

```latex
\maketitle
```

Ejemplo:

```latex
\begin{document}

\maketitle

Contenido del documento.

\end{document}
```

---

# 🗂️ Estructura de Secciones

LaTeX organiza el contenido automáticamente mediante comandos jerárquicos.

| Comando | Función |
|---|---|
| `\section{...}` | Sección principal |
| `\subsection{...}` | Subsección |
| `\subsubsection{...}` | Subdivisión adicional |

Ejemplo:

```latex
\section{Introducción}

\subsection{Antecedentes}

\subsubsection{Historia}
```

Si deseas una sección sin numeración:

```latex
\section*{Conclusión}
```

---

# 🧩 Ejemplo Completo de Código

```latex
\documentclass{article}

% --- Preámbulo ---
\title{Mi Primer Proyecto}
\author{Nombre del Autor}
\date{\today}

\begin{document}

\maketitle % Genera el título

\section{Introducción}
Este es un ejemplo de cómo estructurar un documento básico.

\subsection{Antecedentes}
LaTeX facilita la organización mediante secciones y subsecciones automáticas.

\end{document}
```

---

# 🏗️ Estructura y Configuración

## `\documentclass{...}`

Define la clase del documento (`article`, `report`, `book`, etc.).

```latex
\documentclass{report}
```

---

## `\usepackage{...}`

Carga paquetes externos para añadir funcionalidades.

```latex
\usepackage{graphicx}
\usepackage{amsmath}
```

Paquetes comunes:

| Paquete | Función |
|---|---|
| `graphicx` | Insertar imágenes |
| `amsmath` | Matemáticas avanzadas |
| `geometry` | Configurar márgenes |
| `babel` | Soporte para idiomas |

---

## `\begin{document}` y `\end{document}`

Delimitan el contenido visible del documento.

```latex
\begin{document}

Contenido

\end{document}
```

---

## `\tableofcontents`

Genera automáticamente el índice.

```latex
\tableofcontents
```

---

# 🏷️ Información del Título

## `\title{...}`

```latex
\title{Mi Documento}
```

## `\author{...}`

```latex
\author{Juan Pérez}
```

## `\date{...}`

```latex
\date{\today}
```

## `\thanks{...}`

Agrega notas al pie en el autor.

```latex
\author{Juan Pérez \thanks{Universidad UDE}}
```

## `\maketitle`

Muestra título, autor y fecha.

```latex
\maketitle
```

---

# ✍️ Formato de Texto y Comentarios

| Comando | Función |
|---|---|
| `\textbf{...}` | Negrita |
| `\textit{...}` | Cursiva |
| `\underline{...}` | Subrayado |
| `\emph{...}` | Énfasis |
| `%` | Comentarios |

Ejemplos:

```latex
\textbf{Texto en negrita}

\textit{Texto en cursiva}

\underline{Texto subrayado}

% Esto es un comentario
```

Salto de línea:

```latex
Texto línea 1 \\
Texto línea 2
```

o

```latex
Texto línea 1
\newline
Texto línea 2
```

---

# 🧱 Organización del Contenido

```latex
\section{...}
\subsection{...}
\subsubsection{...}
```

Sección sin numeración:

```latex
\section*{Bibliografía}
```

Solo para `report` y `book`:

```latex
\chapter{Capítulo 1}

\part{Parte I}
```

---

# 🖼️ Elementos Visuales y Referencias

## Insertar imágenes

```latex
\includegraphics{imagen.png}
```

(Requiere `graphicx`)

---

## Títulos para imágenes y tablas

```latex
\caption{Descripción de la imagen}
```

---

## Etiquetas y referencias

```latex
\label{fig:ejemplo}

\ref{fig:ejemplo}
```

---

# 📋 Listas y Tablas

## Lista con viñetas

```latex
\begin{itemize}
\item Primer elemento
\item Segundo elemento
\end{itemize}
```

---

## Lista numerada

```latex
\begin{enumerate}
\item Paso uno
\item Paso dos
\end{enumerate}
```

---

## Tablas

```latex
\begin{tabular}{|c|c|}
\hline
Nombre & Edad \\
\hline
Juan & 20 \\
\hline
\end{tabular}
```

| Símbolo | Función |
|---|---|
| `&` | Separar columnas |
| `\\` | Terminar fila |
| `\hline` | Línea horizontal |

---

# ➗ Matemáticas

## Matemáticas en línea

```latex
$ a^2 + b^2 = c^2 $
```

o

```latex
\( a^2 + b^2 = c^2 \)
```

---

## Matemáticas en bloque

```latex
\[
a^2 + b^2 = c^2
\]
```

o

```latex
\begin{equation}
a^2 + b^2 = c^2
\end{equation}
```l modo matemático en pantalla para ecuaciones que ocupan su propia línea.
