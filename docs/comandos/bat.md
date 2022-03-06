# bat

Imprima e concatene arquivos. Um clone do comando `cat` com destaque da sintaxe e integração do git. 



## Exemplos


Saida do comando: `tldr bat`


```
bat
Print and concatenate files.A cat clone with syntax highlighting and Git integration.More information: https://github.com/sharkdp/bat.

 - Print the contents of a file to the standard output:
   bat {{arquivo}}

 - Concatenate several files into the target file:
   bat {{file1}} {{file2}} > {{target_file}}

 - Append several files into the target file:
   bat {{file1}} {{file2}} >> {{target_file}}

 - Number all output lines:
   bat -n {{arquivo}}

 - Syntax highlight a json file:
   bat --language json {{file.json}}

 - Display all supported languages:
   bat --list-languages
```