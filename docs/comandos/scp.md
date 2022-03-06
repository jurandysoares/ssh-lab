# scp

Cópia segura.Copie arquivos entre hosts usando o protocolo *Secure Copy Protocol* sobre SSH.

## Exemplos

Saida do comando: `tldr scp`


```
scp
Secure copy.Copy files between hosts using Secure Copy Protocol over SSH. 

 - Copie um arquivo local para um host remoto:
   scp {{caminho/para/arquivo_local}} {{host_remoto}}:{{caminho/para/arquivo_remoto}}

  - Copie um arquivo de um host remoto para um diretório local:
   scp {{host_remoto}}:{{caminho/para/arquivo_remoto}} {{caminho/para/diretorio_local}}

 - Copie recursivamente o conteúdo de um diretório de um host remoto para um diretório local:
   scp -r {{host_remoto}}:{{caminho/para/diretorio_remoto}} {{caminho/para/diretorio_local}}
```