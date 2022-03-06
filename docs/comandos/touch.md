# touch

Altere um acesso a arquivos e horários de modificação (atime, mtime).

É muito utilizado para criar arquivos vazios.

## Exemplos


Saida do comando: `tldr touch`


```
touch
Change a file access and modification times (atime, mtime).

 - Create a new empty file(s) or change the times for existing file(s) to current time:
   touch {{filename}}

 - Set the times on a file to a specific date and time:
   touch -t {{YYYYMMDDHHMM.SS}} {{filename}}

 - Use the times from a file to set the times on a second file:
   touch -r {{filename}} {{filename2}}
```

```