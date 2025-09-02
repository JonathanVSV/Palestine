# Palestina

## Instrucciones para actualizar libro html

Ese html trae la página web del libro.

El flujo de trabajo normalmente sería:
1. Modificar los archivos qmd. Básicamente son los archivos que se renderean a html. Es muy similar al markdown y usan casi la misma sintaxis.
2. Correr `quarto render` en la terminal para actualizar los archivos html.
3. Revisar el html en docs/index.html

## Estructura del libro

- El archivo _quarto.yml contiene toda la información para crear el libro. Aquí se ponen los autores, título del libro, portada, links, capítulos del libro, etc.
- Luego vienen los archivos individuales de los capítulos empezando por index.qmd y luego van todos los enumerados. Para que todos estos archivos aparezcan en el libro tienen que estar llamados en _quarto.yml