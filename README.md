# Template de Tesis Universidad de Valparaíso

Este es el Template de tesis diseñado para el programa de Doctorado en Ciencias e Ingeniería para la Salud, de la Universidad de Valparaíso, Chile.
Basado en el template LaTeX thesis de [Matthias Pospiech](https://www.matthiaspospiech.de/latex/templates/thesis/).

### Elementos Pendientes
- Bibliografia
- Apendices
- Configuracion del estilo
- Agradecimientos
- Documentación

## Requerimientos
Solo ha sido probado a nivel local, para compilar estamos utilizando LuaLaTeX, por lo que inicialmente uno debiera configurar el compilador de LaTeX para esto (en overleaf en el menu, esta la opcion de usar pdflatex, xelatex y lualatex).

## Metodo de uso
### Configuración
La distribucion del documento esta definida en `main.tex`
Algunas configuraciones se encuentran en la carpeta `preamble`, donde estan definidos los paquetes (`packages.tex`), la fuente a utilizar (`fonts.tex`), algunos parametros del diseño (`styles.tex`), etc.

### Archivos
Dentro de la carpeta `elements`, se incluyen la tipografía oficial de la Universidad (Swiss721 BT), junto con el logo en formato vectorial (`.eps`)

### Bibliografía
Para la bibliografía, se utiliza `biblatex`. Los archivos .bib deben insertarse en la carpeta `bib/` y en el archivo main, debe añadirse cada archivo con `\addbibresource{bib/referencia.bib}` donde referencia.bib es el archivo.

