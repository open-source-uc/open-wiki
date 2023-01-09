# C

Puedes consultar el apartado de [configuraciones](./configuraciones.md) para su funcionamiento.

## Talleres

- [Intro a C por Vicente Errázuriz y Raúl Álvarez](https://github.com/DCCentral-de-Apuntes/intro-C)

- [Capsula de Debugging en GDB](https://youtu.be/RNfVQQEUoMQ)

## Configuraciones

Aca se encuentran algunas recomendaciones sobre las configuraciones iniciales.

### VScode

Siguiendo la guia de [VScode](../../herramientas/vscode.md). Pueden incluir en las configuraciones de vscode lo siguiente ++ctrl+shift+p++ o ++f1++:

```json
	 // C
    "files.associations": {
        "process.h": "c"
    },
    "C_Cpp.clang_format_fallbackStyle": "Google",
    "C_Cpp.clang_format_style": "{ BasedOnStyle: Google, IndentWidth: 2, ColumnLimit: 0, IndentCaseLabels: false, TabWidth: 2, SpacesBeforeTrailingComments: 3, BreakBeforeBraces: Custom, BraceWrapping: { BeforeElse: false } }",
```
