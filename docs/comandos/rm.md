# rm

Remova arquivos ou diretórios.

## Exemplos


Saida do comando: `tldr rm`


```
rm
Remove files or directories.

 - Remove files from arbitrary locations:
   rm {{caminho/para/arquivo}} {{caminho/para/outro/arquivo}}

 - Recursively remove a directory and all its subdirectories:
   rm -r {{caminho/para/diretorio}}

 - Forcibly remove a directory, without prompting for confirmation or showing error messages:
   rm -rf {{caminho/para/diretorio}}

 - Interactively remove multiple files, with a prompt before every removal:
   rm -i {{arquivo(s)}}

 - Remove files in verbose mode, printing a message for each removed file:
   rm -v {{caminho/para/diretorio/*}}
```
