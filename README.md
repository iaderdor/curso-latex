# Curso de Introducción a LaTeX

Este repositorio contiene los ejemplos con los que se trataron en el Curso de Introducción a LaTeX impartido por la Biblioteca de Ciencias Físicas de la Universidad Complutense de Madrid y ASAAF-UCM los días 3 y 5 de abril de 2017.

Además, se incluyen también algunas de las instrucciones que se explicaron durante el curso.


## Contenido

El objetivo del curso es enseñar a estudiantes de Físicas a usar LaTeX a un nivel básico. Se pretende que tras realizar el curso, el participante pueda comenzar a realizar proyectos mediante esta herramienta.

Los contenidos del curso fueron:


### Primera sesión

 * Compilación de archivos de LaTeX
 * Declaración de la clase del documento. Diferencias básicas entre `book`, `report` y `article`. Parámetros requeridos por `\documentclass`
 * Estructura de los comandos y ambientes de LaTeX.
 * Preámbulo y cuerpo del documento. Uso del ambiente `document`. Realización de comentarios.
 * Estructura del documento. Partes, capítulos, secciones, subsecciones, párrafos. Creación de índice.
 * Definición del título. Uso de plantillas para crear títulos.
 * Carga de paquetes. Paquetes recomendados.
 * Elementos deslizantes. Declaración de figuras y parámetros. Colocadores. El paquete `float`. Inclusión de imágenes. Pie de foto.
 * Etiquetas y referencias. Situación de etiquetas. Recomendaciones a la hora de nombrar etiquetas.
 * Realización de tablas. Asistente para tablas de TeXmaker.
 * Ambiente matemático. Ecuaciones destacadas y en línea. Numeración de ecuaciones.

### Segunda sesión

 * Ambiente matemático. Diferencias entre ecuaciones destacadas y en línea. Formateo de texto en ambiente matemático. Espacios en modo matemático.
 * Uso de bibtex. Generación de base de datos con la bibliografía. Estilos de bibliografía. Generación de citas.
 * Definición de comandos personalizados.
 * Organización del documento. Separación de paquetes, comandos y títulos del documento maestro. Paquete `subfiles`. Separación de los archivos `.tex` según la estructura del documento.
 * Paquetes de la AMSLaTeX: `amsmath`, `amssymbol`, `amsfonts`. Matrices. Paréntesis, corchetes, llaves y similar dentro de ecuaciones. Los ambientes `gather`, `align`, `aligned`, `cases` y `subequations`.


## Instalación de LaTeX

La instalación dependerá del sistema operativo que estemos usando. Existen varias distribuciones de LaTeX, así como editores, pero durante el curso usaremos `texlive` y `TeXmaker`. Esto es una cuestión completamente personal, sobre todo en lo referente a editores. Para el curso hicimos esta elección debido a que los tres son programas de software libre, que tienen una base de usuarios amplia (con lo cual es más sencillo encontrar la respuesta a las dudas que uno se encuentre buscando en internet) y que además están disponibles para los sistemas operativos mayoritarios.

### Instalación en Windows

Para instalar `texlive` en Windows deberemos descargarnos en primer lugar el [instalador](http://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe) de la [página web de TUG](https://www.tug.org/texlive) (TeX User Group). Una vez descargado, abrimos el instalador y seguimos los pasos. Hay que asegurarse de instalar todos los paquetes y de seleccionar una ruta de instalación con la que nos sintamos cómodos. Una vez realizados estos pasos, le damos a instalar y el programa se encargará de descargar e instalar todos los paquetes necesarios.

Ten en cuenta que la instalación completa de `TeXLive` ocupa alrededor de 4600MB y que debe descargar todo de internet, con lo cual en función de la conexión que tengas puede tardar bastante tiempo.

Finalmente, nos resta instalar TeXmaker. Procederemos descargándolo de [aquí](http://www.xm1math.net/texmaker/), seleccionando la versión adecuada para Windows. Finalmente, ejecutamos el instalador y seguimos los pasos que nos indique.

### Instalación en Linux

Para instalar `texlive` en linux es más sencillo usar directamente el gestor de paquetes de la distribución que usemos. Los comandos a usar dependen de la distro que se use:

 * Ubuntu, debian y derivados: `apt-get install texlive-full`
 * OpenSuse: `zypper install texlive`
 * Archlinux y Manjaro: `pacman -S texlive-most`
 * Fedora: `dng install texlive texlive-scheme-full`

Recuerda que para poder instalar estos paquetes se necesitan permisos de superusuario. Tras ejecutar el comando, el gestor de paquetes descargará e instalará `TeXlive`. Ten en cuenta que la instalación ocupa en torno a 4GB, con lo cual tardará un rato en instalarlo.

Finalmente, para instalar `TeXmaker` es recomendable usar también el gestor de paquetes. En este caso, en todas las distribuciones el paquete se llama `texmaker`.

Si usas una distribución que no esté nombrada aquí, es muy probable que no tenga que mencionarte como usar el gestor de paquetes. Simplemente, asegurate que el `texlive` que instales sea el que tiene todos los paquetes de LaTeX.


### Instalación en OS/X

Para instalar `TeXlive` en OSX, primeramente debemos descargar la distribución específica para OSX, llamada MacTeX. El nombre es distinto, pero el software es el mismo. Puede descargarse también desde la [página web del TUG](https://tug.org/mactex/mactex-download.html). El archivo a descargar pesa 2.4GB, así que tardará un rato en descargarse. Finalizada la descarga, ejecuta el instalador y sigue las instrucciones.

Finalmente, nos resta instalar TeXmaker. Procederemos descargándolo de [aquí](http://www.xm1math.net/texmaker/), seleccionando la versión adecuada para OS/X. Finalmente, ejecutamos el instalador y seguimos los pasos que nos indique.


## Bibliografía

A continuación añado algunos documentos que creo que pueden ser de utilidad para seguir aprendiendo a manajar LaTeX.

 * [The not so short introduction to LaTeX2e](http://osl.ugr.es/CTAN/info/lshort/english/lshort.pdf): Este es un libro bastante corto en el que te enseñan a usar LaTeX desde cero. Toca algunos temas que no hemos usado, como los carácteres reservados, cómo trata LaTeX los espacios. El tema 3 trata bastante más en profundidad el ambiente matemático en comparación con cómo lo hemos visto en el curso. El tema 5 también tiene una ligerilla introducción a cómo realizar graficos, pero es muy escueta. Puede encontrarse también este libro en español, pero no suele estar tan actualizado.
 * [Guía casi completa de bibTeX](ftp://ftp.dante.de/tex-archive/documentation/spanish/guia-bibtex/guia-bibtex.pdf): Este documento es un compendio bastante grande acerca del uso de `bibtex`.
 * [TikZ & PGF](http://osl.ugr.es/CTAN/graphics/pgf/base/doc/pgfmanual.pdf): La "biblia" de `TikZ`. Es un manual escrito por el autor del paquete en el que enseña a usar la herramienta mediante tutoriales. Tiene también una parte que es completamente un manual de referencia.

En caso de querer buscar el funcionamiento de un paquete concreto, en la página del [CTAN](https://www.ctan.org/) suele existir casi siempre documentación al respecto. Por lo general, la documentación es decente, pero a veces sólo está completamente actualizada en alemán o bien es bastante escueta. Sin embargo, al tener una duda concreta de cómo realizar algo se puede realizar una búsqueda en google para comprobar si hay alguien que haya tenido el mismo problema que nosotros. En caso de no encontrar la solución al problema, siempre se puede preguntar en [stackexchange](http://tex.stackexchange.com/) o en [reddit](https://www.reddit.com/r/LaTeX/).


Como referencia a la hora de rellenar algunos de los comandos de LaTeX, os añado a continuación algunos sitios en donde podéis encontrar más información con la que rellenar los comandos:

 * [Estructura del documento](https://en.wikibooks.org/wiki/LaTeX/Document_Structure): Aquí se encuentran las principales clases de documentos que existen en LaTeX. Tiene también las opciones que se pueden añadir, así como los distintos comandos para estructurar documentos.
 * [Plantillas de LaTeX](https://www.latextemplates.com/): Esta página tiene muchas plantillas de LaTeX listas para ser usadas.
 * [Estilos de bibliografía](https://es.sharelatex.com/learn/Bibtex_bibliography_styles): Una pequeña muestra de los distintos estilos de bibliografía que pueden usarse. En [esta respuesta](http://tex.stackexchange.com/a/35047) hay un link a 4 páginas que contienen bastantes estilos de bibliografía.
