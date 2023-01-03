# Configuraciones

Aca se encuentran algunas recomendaciones sobre las configuraciones iniciales.

## VScode

Siguiendo la guia de [VScode](.../Herramientas/vscode.md). Pueden incluir en las configuraciones de vscode lo siguiente (`ctrl+shif+p` p `F1`):

=== "flake8"
    ```json
        // -------------- LINTER ----------------
        // PEP8
        "editor.rulers": [100],
        "python.linting.enabled": true,
        // flake8
        "python.linting.pylintEnabled": false,
        "python.linting.flake8Enabled": true,
        "python.formatting.provider": "black",
        "python.formatting.blackArgs": [
            "--line-length",
            "100"
        ],
        "python.linting.flake8Args": [
            "--max-line-length=100",
            "--ignore=F841,F401,E302,E305",
        ],
    ```
=== "pycodestyle"
    ```json
        // -------------- LINTER ----------------
        // PEP8
        "editor.rulers": [100],
        "python.linting.enabled": true,
        // pycodestyle
        "python.linting.pycodestyleArgs": [
            "--max-line-length=100"
        ],
    ```


Aca se presentan varias opciones para el linter. Lo importante es que luego de guardar, tendran que reiniciar y al abrir un .py les va a salir una ventana de instalacion que tienen que aceptar. Si no, lo tendran que hacer manualmente buscando en internet dependiendo de la guia de estilo que deseen.