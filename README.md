# Template de Tesis Universidad de Valparaíso

Este es el Template de tesis diseñado para el programa de Doctorado en Ciencias e Ingeniería para la Salud, de la Universidad de Valparaíso, Chile.
Basado en el template LaTeX thesis de [Matthias Pospiech](https://www.matthiaspospiech.de/latex/templates/thesis/).

### Elementos Pendientes
- Apendices
- Configuracion del estilo
- Agradecimientos
- Documentación

## Requerimientos
Solo ha sido probado a nivel local, para compilar estamos utilizando LuaLaTeX, por lo que inicialmente uno debiera configurar el compilador de LaTeX para esto (en overleaf en el menu, esta la opcion de usar pdflatex, xelatex y lualatex).

### Algunos paquetes utilizados
- siunitx: unidades
- biblatex: manejo de bibliografia
- biblatex-vancouver: Formato Vancouver para biblatex (_no cumple 100%? aproxima al estilo_)
- floatrow: manejo de objetos flotantes para figuras, tablas, etc
- wrapfig
- glossaries: manejo de glosario


## Metodo de uso

En el capitulo 3 (Metodologia), carga el archivo [`example.tex`](content/template/example.tex), en donde se presentan algunos elementos básicos para presentar, tales como figuras, tablas, entre otros.

### Configuración
La distribucion del documento esta definida en [`main.tex`](main.tex)
Algunas configuraciones se encuentran en la carpeta `preamble`, donde estan definidos los [paquetes](preamble/packages.tex), la [fuente a utilizar](preamble/fonts.tex), algunos parametros del [diseño](preamble/styles.tex), etc.

### Archivos
Dentro de la carpeta `elements`, se incluyen la tipografía oficial de la Universidad (Swiss721 BT), junto con el logo en formato vectorial (`.eps`)

### Bibliografía
Para la bibliografía, se utiliza `biblatex`. Los archivos .bib deben insertarse en la carpeta `bib/` y en el archivo main, debe añadirse cada archivo con `\addbibresource{bib/referencia.bib}` donde referencia.bib es el archivo.

En el caso de los glosarios y definiciones de acronimos, estos se definen dentro del archivo [`ZZ-Glossary.tex`](content/ZZ-Glossary.tex). Teoricamente, deberia compilar directamente el glosario con la ejecución de latexmk (parametros definidos en el archivo [`latexmkrc`](.latexmkrc))
Si no fuese el caso, uno debiese ejecutar en consola el comando `makeglossaries [archivo]`.