# cat

Imprima e concatene arquivos.

## Exemplos


Saida do comando: `tldr cat`


```
cat
Print and concatenate files.

 - Print the contents of a file to the standard output:
   cat {{file}}

 - Concatenate several files into the target file:
   cat {{file1}} {{file2}} > {{target_file}}

 - Append several files into the target file:
   cat {{file1}} {{file2}} >> {{target_file}}

 - Number all output lines:
   cat -n {{file}}

 - Display non-printable and whitespace characters (with M- prefix if non-ASCII):
   cat -v -t -e {{file}}
```