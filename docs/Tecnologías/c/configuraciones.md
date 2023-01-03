# Configuraciones

Aca se encuentran algunas recomendaciones sobre las configuraciones iniciales.

## VScode

Siguiendo la guia de [VScode](../Herramientas/vscode.md). Pueden incluir en las configuraciones de vscode lo siguiente (`ctrl+shif+p` p `F1`):

```json
	 // C
    "files.associations": {
        "process.h": "c"
    },
    "C_Cpp.clang_format_fallbackStyle": "Google",
    "C_Cpp.clang_format_style": "{ BasedOnStyle: Google, IndentWidth: 2, ColumnLimit: 0, IndentCaseLabels: false, TabWidth: 2, SpacesBeforeTrailingComments: 3, BreakBeforeBraces: Custom, BraceWrapping: { BeforeElse: false } }",
```
