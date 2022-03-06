# scp

Cópia segura.Copie arquivos entre hosts usando o protocolo *Secure Copy Protocol* sobre SSH.

## Exemplos

Saida do comando: `tldr scp`


```
scp
Secure copy.Copy files between hosts using Secure Copy Protocol over SSH. 

 - Copy a local file to a remote host:
   scp {{path/to/local_file}} {{remote_host}}:{{path/to/remote_file}}

  - Copy a file from a remote host to a local directory:
   scp {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}

 - Recursively copy the contents of a directory from a remote host to a local directory:
   scp -r {{remote_host}}:{{path/to/remote_directory}} {{path/to/local_directory}}
```