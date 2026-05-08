# LaTeX
LaTeX es una herramienta para la composición de documentos de aspecto profesional que funciona mediante comandos de texto plano, permitiéndote enfocarte en el contenido mientras el sistema se encarga de la apariencia visual.

1. Definición de la Clase del Documento
Todo documento de LaTeX debe comenzar declarando su clase, la cual controla el diseño general. Para documentos estándar, se utiliza la clase article.
\documentclass{article}

2. El Preámbulo y la Configuración del Título
El preámbulo es la sección de configuración que aparece antes del inicio del cuerpo del documento. Aquí se define la información que aparecerá en el título:
\title{...}: Título del documento.
\author{...}: Nombre del autor.
\date{...}: Fecha manual o el comando \today para usar la fecha actual de compilación.

3. Cuerpo del Documento
El contenido visible se escribe dentro del entorno del cuerpo, delimitado por las etiquetas \begin{document} y \end{document}. Para que el título configurado en el preámbulo aparezca en el PDF, se debe insertar el comando \maketitle al inicio del cuerpo.

4. Estructura de Secciones
Para organizar el contenido de manera jerárquica, LaTeX ofrece comandos de seccionamiento que se numeran de forma automática:
\section{...}: Sección principal.
\subsection{...}: Subdivisión de una sección.
\subsubsection{...}: División adicional de una subsección.
Nota: Si deseas una sección sin numeración, puedes usar la versión con asterisco: \section*{Nombre}.

--------------------------------------------------------------------------------
Ejemplo Completo de Código
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
