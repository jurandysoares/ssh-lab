# nano

Simples, fácil de usar o editor de texto de linha de comando. Um clone do pico, melhorado e gratuito.

## Exemplos

Saída do comando: `tldr nano`

```
 - Open a new file in nano:
   nano

 - Open a specific file:
   nano {{caminho/para/arquivo}}

 - Open a specific file, positioning the cursor at the specified line and column:
   nano +{{line}},{{column}} {{caminho/para/arquivo}}

 - Open a specific file and enable soft wrapping:
   nano --softwrap {{caminho/para/arquivo}}

 - Open a specific file and indent new lines to the previous lines' indentation:
   nano --autoindent {{caminho/para/arquivo}}

 - Open nano and create a backup file (file~) when saving edits:
   nano --backup {{caminho/para/arquivo}}
```