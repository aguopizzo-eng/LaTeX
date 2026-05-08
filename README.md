# LaTeX
LaTeX es una herramienta para la composición de documentos de aspecto profesional que funciona mediante comandos de texto plano, permitiéndote enfocarte en el contenido mientras el sistema se encarga de la apariencia visual.

1. Definición de la Clase del Documento:
Todo documento de LaTeX debe comenzar declarando su clase, la cual controla el diseño general. Para documentos estándar, se utiliza la clase article.
\documentclass{article}

2. El Preámbulo y la Configuración del Título:
El preámbulo es la sección de configuración que aparece antes del inicio del cuerpo del documento. Aquí se define la información que aparecerá en el título:
\title{...}: Título del documento.
\author{...}: Nombre del autor.
\date{...}: Fecha manual o el comando \today para usar la fecha actual de compilación.

3. Cuerpo del Documento:
El contenido visible se escribe dentro del entorno del cuerpo, delimitado por las etiquetas \begin{document} y \end{document}. Para que el título configurado en el preámbulo aparezca en el PDF, se debe insertar el comando \maketitle al inicio del cuerpo.

4. Estructura de Secciones:
Para organizar el contenido de manera jerárquica, LaTeX ofrece comandos de seccionamiento que se numeran de forma automática:
\section{...}: Sección principal.
\subsection{...}: Subdivisión de una sección.
\subsubsection{...}: División adicional de una subsección.
Nota: Si deseas una sección sin numeración, puedes usar la versión con asterisco: \section*{Nombre}.

--------------------------------------------------------------------------------
Ejemplo Completo de Código:
Puedes usar este código como base para tu primer archivo .tex:
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


Estructura y Configuración
\documentclass{...}: Define la clase del documento (como article, report o book), lo que controla el diseño general.
\usepackage{...}: Carga paquetes externos para añadir funciones especiales, como graphicx para imágenes o amsmath para matemáticas avanzadas.
\begin{document} y \end{document}: Delimitan el cuerpo del documento; todo lo que esté fuera de estas etiquetas no se mostrará en el PDF.
\tableofcontents: Genera automáticamente el índice del documento basándose en las secciones creadas.
Información del Título (Preámbulo)
\title{...}, \author{...} y \date{...}: Definen los metadatos del documento.
\thanks{...}: Añade una nota al pie (como un agradecimiento) dentro del comando de autor.
\maketitle: Comando necesario dentro del cuerpo del documento para que el título, autor y fecha aparezcan realmente en el PDF.
Formato de Texto y Comentarios
\textbf{...}: Aplica negrita al texto.
\textit{...}: Aplica cursiva.
\underline{...}: Subraya el texto.
\emph{...}: Enfatiza el texto (generalmente en cursiva, pero su comportamiento varía según el contexto).
%: Se utiliza para añadir comentarios en el código; todo lo que siga a este símbolo en la misma línea no será procesado por LaTeX.
\\ o \newline: Inserta un salto de línea manual sin comenzar un nuevo párrafo.
Organización del Contenido
\section{...}, \subsection{...}, \subsubsection{...}: Crean divisiones jerárquicas numeradas automáticamente.
\section*{...}: Crea una sección sin numerar.
\chapter{...} y \part{...}: Comandos de organización disponibles únicamente en las clases report y book.
Elementos Visuales y Referencias
\includegraphics{...}: Inserta una imagen en el documento (requiere el paquete graphicx).
\caption{...}: Añade un título descriptivo a una imagen (figura) o tabla.
\label{...} y \ref{...}: Permiten etiquetar un elemento y referenciarlo numéricamente en cualquier otra parte del texto.
Listas y Tablas
itemize: Entorno para crear listas con viñetas (no numeradas).
enumerate: Entorno para crear listas numeradas.
\item: Indica el inicio de un nuevo elemento dentro de una lista.
tabular: Entorno para crear tablas, donde se usa & para separar columnas y \\ para terminar filas.
\hline: Dibuja una línea horizontal dentro de una tabla.
Matemáticas
$ ... $ o \( ... \): Activa el modo matemático en línea (dentro de un párrafo).
\[ ... \] o el entorno equation: Activa el modo matemático en pantalla para ecuaciones que ocupan su propia línea.
