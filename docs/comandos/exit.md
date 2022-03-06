# exit

Saia da interpretador de comandos (*Shell*).

## Exemplos


Saida do comando: `tldr exit`


```
exit
Exit the shell.

 - Exit the shell with the exit code of the last command executed:
   exit

 - Exit the shell with the specified exit code:
   exit {{exit_code}}
```
## Diagrama de sequência

```mermaid
sequenceDiagram
    autonumber
    participant cli as Cliente<br>SSH
    participant srv as Servidor<br>SSH

    cli ->> srv: Cliente inicia uma conexão contactando o servidor
    srv -->> cli: Envia chave pública do servidor
    cli ->> srv: Negocia parâmetros e abre um canal seguro
    cli ->> srv: Envia usuário
    srv -->> cli: Solicita senha
    cli ->> srv: Envia senha
    srv -->> cli: Autentica usuário e libera terminal remoto
    cli ->> srv: exit
    srv -->> cli: Encerra sessão.
```
