# ssh

O Secure Shell é um protocolo usado para efetuar login no sistema remoto. Pode ser usado para registrar ou executar comandos em um servidor remoto.

## Exemplos

Saida do comando: `tldr ssh`

```
ssh
Secure Shell is a protocol used to securely log onto remote systems.It can be used for logging or executing commands on a remote server.

 - Connect to a remote server:
   ssh {{username}}@{{remote_host}}

 - Run a command on a remote server:
   ssh {{remote_host}} {{command -with -flags}}

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
```