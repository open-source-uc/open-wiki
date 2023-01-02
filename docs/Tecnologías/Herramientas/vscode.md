# ¿Que es VSCode?
Visual Studio Code (VSCode) es un editor de código fuente gratuito y de código abierto desarrollado por Microsoft. Es compatible con diversos lenguajes de programación y ofrece una amplia gama de características para facilitar el desarrollo de aplicaciones.

# Características principales
- IntelliSense: VSCode ofrece autocompletado y sugerencias de código para varios lenguajes de programación.
- Depuración: VSCode incluye herramientas de depuración para ayudar a encontrar y solucionar errores en el código.
- Git integrado: VSCode incluye funcionalidades de control de versiones integradas para trabajar con repositorios Git.
- Extensiones: VSCode cuenta con una gran cantidad de extensiones disponibles para personalizar y ampliar sus funcionalidades.

# Descarga e instalación
VSCode se puede descargar de forma gratuita desde la página web oficial de Microsoft: https://code.visualstudio.com/. La instalación es sencilla y seguir las instrucciones del asistente de instalación.

# Configuración

Al principio puede parecer extraño, pero todas las configuraciones de vscode estan en un archivo `.json` que pueden personalizar. Para ingresar a el tienen que teclear `[CTRL] + [SHIFT] + P` o `F1` y escribir `Preferencias: Abrir Configuración (JSON)` o `Preferences: Open Settings (JSON)` Si lo tienen en ingles.

Como ejemplo. Pueden pegar las siguientes lineas dentro de los "{}", solo procura que la ultima linea que agregues al archivo no tenga la coma puesta:

```json
// Limite de largo en las lineas, en avanzada se permiten 100
"python.linting.pycodestyleArgs": ["--max-line-length=100"],
"editor.rulers": [100],
// Al guardar ordena el codigo al estilo deseado (linter)
"editor.formatOnSave": true,
```

# Atajos de teclado
Si quieres ver todos los atajos, puedes presionar `Ctrl + K + S` para ver la lista completa de atajos de teclado disponibles.
En windows se utiliza `CTRL`y en mac `CMD`, pero en general funcionan igual.

- COMENTAR varias líneas y a la vez: `[CTRL] + K` (Vscode queda a la espera). Después pulsa `[CTRL] + C` para comentar y `[CTRL] + U` para descomentar.
- `Ctrl + Shift + L` Selecciona todas las ocurrencias de la selección actual.
- `Ctrl + S`: Guarda el archivo actual.
- `Ctrl + Shift + S`: Guarda todos los archivos abiertos.
- `Ctrl + W`: Cierra el archivo actual.
- `Ctrl + Shift + W`: Cierra todos los archivos abiertos.
- `Ctrl + F`: Abre la barra de búsqueda.
- `Ctrl + P`: Muestra el panel de navegación de archivos.


# Extensiones utiles

- *Code Runer*: Te permite ejecutar el código de forma mucho más amigable sin escribir en la consola.
- *Spanish Language Pack*: Te permite tener VSCode en español.
- *Project Manager*: Sirve para tener carpetas en favoritos y para no perder el tiempo buscando en las carpetas.
- *Better Commets*: Agrega opciones para comentarios con colores, es SUPER recomendada.
- *Jupyter Extension*: Te permite integrar Jupyter en el editor, es MUY cómodo y te permite desplazarte de forma muy amigable entre carpetas.
- *Draw.io Integration*: Sirve para hacer diagramas de draw.io desde el mismo VSCode.


# Temas de color recomendados
_Recomiendamos evitar themes que tengan alto contraste como Monokai Charcoal o Pitch Black._

- *One Dark Pro*: Es de los temas más instalados y es agradable para usar durante varias horas de trabajo.
- *Polykai*: Un tema oscuro con buen contraste
- *Dracula Official*: Tiene colores muy agradables

# Tipografias recomendadas

- *JetBrains Mono*: Una tipografía muy utilizada y que permite activar 'ligaduras' para formar símbolos y flechas (recomiendo buscar un tutorial para instalarlo).

