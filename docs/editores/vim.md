# vim

Vim (vi melhorado), um editor de texto de linha de comando, fornece vários modos para diferentes tipos de manipulação de texto. Pressionar `i` entra no modo Inserir. `<ESC>` entra no modo normal, que permite o uso de comandos do vim.

## Exemplos

Saída do comando: `tldr vim`

```
 - Abrir um arquivo:
   vim {{caminho/para/arquivo}}

 - Abrir um arquivo at a specified line number:
   vim +{{line_number}} {{caminho/para/arquivo}}

 - View Vim's help manual:
   :help<Enter>

 - Save and Quit:
   :wq<Enter>

 - Undo the last operation:
   u

 - Search for a pattern in the file (press n/N to go to next/previous match):
   /{{search_pattern}}<Enter>

 - Perform a regular expression substitution in the whole file:
   :%s/{{regular_expression}}/{{replacement}}/g<Enter>

 - Display the line numbers:
   :set nu<Enter>
```