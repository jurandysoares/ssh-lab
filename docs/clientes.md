# Clientes

Em distribuições Linux e no Mac OS é comum vir um cliente SSH, que pode facilmente ser chamado pelo terminal.

No Windows, o terminal do Git Bash, que é instalado junto com o [Git para Windows](https://git-scm.com/download/win), oferece os mesmos comandos do cliente SSH que estão disponíveis no Linux e no Mac OS.

Os comandos principais são:

- `ssh`: Estabelece uma conexão com dois tipos possíveis de sessão:

    - login
    - não interativa 
      
    Para este laboratório, vamos utilizar somente a interativa.

- `ssh-keygen`: Comando que gera par de chaves pública/privada para o usuário. O GitHub tem uma excelente documentação em português a respeito. Veja: [Gerar uma nova chave SSH e adicioná-la ao ssh-agent - GitHub Docs](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).
- `ssh-copy-id`: Permite copiar uma chave pública de seu usuário na máquina local para o conjunto de chaves autorizadas para seu usuário em um servidor remoto. Ele é util, por exemplo, para permitir o acesso remoto sem a solicitação de senha.

Caso queira um cliente SSH mais amistoso, com interface gráfica, uma ótima solução é o MobaXterm:

- [MobaXterm Xserver with SSH, telnet, RDP, VNC and X11 - Download](https://mobaxterm.mobatek.net/download.html)
