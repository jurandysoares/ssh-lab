# Comandos

!!! note "Algumas palavras sobre mouse e o foco"

    > Embora o shell seja totalmente voltado para o teclado, você também pode usar um mouse com o emulador de terminal. Há um mecanismo embutido no sistema X Window (o mecanismo subjacente que faz a interface gráfica do usuário -- `GUI` -- funcionar) que suporta uma técnica rápida de copiar e colar. Se você destacar algum texto mantendo pressionado o botão esquerdo do mouse e arrastando o mouse sobre ele (ou clicando duas vezes em uma palavra), ele é copiado para um buffer mantido por X. Pressionar o botão do meio do mouse fará com que o texto seja colado na localização do cursor. Tente.

    > Nota: Não fique tentado a usar `Ctrl-c` e `Ctrl-v` para copiar e colar dentro de uma janela de terminal. Eles não funcionam. Esses códigos de controle têm diferentes significados para o shell e foram atribuídos muitos anos antes do Microsoft Windows.

    >Fonte: ([The Linux Command Line](https://wiki.lib.sun.ac.za/images/c/ca/TLCL-13.07.pdf), 2013)
```

## Introdução aos comandos do UNIX

O sistema operacional UNIX, do qual o Linux deriva, é freqüentemente considerado um sistema operacional "atômico" -- comandos pequenos, simples e funcionais que podem ser unidos para satisfazer requisitos mais sofisticados do sistema operacional.

Há muito pouca redundância nos comandos UNIX -- em vez de fornecer vários comandos, todos executando funções semelhantes, o UNIX prefere que seus usuários construam seus requisitos a partir de comandos "atômicos" existentes. Voltaremos à junção de comandos mais tarde.

## Estrutura de Comandos UNIX

Para executar um comando em um sistema UNIX, você digita o nome do comando, junto com qualquer informação associada, como um nome de arquivo, e pressiona a tecla `Enter`. A linha digitada é chamada de linha de comando e o UNIX usa um programa especial, chamado shell ou interpretador de linha de comando, para interpretar o que você digitou no que você deseja fazer. Os componentes da linha de comando são:

1. O comando;
2. Quaisquer opções exigidas pelo comando;
3. Os argumentos do comando (se necessário).
   
Por exemplo, a forma geral de um comando UNIX é:

- `comando` `[-opção(ões)]` `[argumento(s)]`

!!! note

    As opções DEVEM vir depois do comando e antes de quaisquer argumentos de comando. As opções NÃO DEVEM aparecer após o(s) argumento(s) principal(is). No entanto, algumas opções podem ter seus próprios argumentos! Historicamente, os comandos do UNIX têm sido razoavelmente padronizados na maneira como usam as opções, mas existem variações -- esteja ciente!


Os novos comandos devem obedecer a uma sintaxe específica regida pelas seguintes regras:

- Os nomes dos comandos devem ter entre 2 e 9 caracteres de comprimento
- Os nomes dos comandos devem ser compostos por caracteres minúsculos e dígitos
- Os nomes das opções devem ter um caractere de comprimento
- Todas as opções são precedidas por um hífen (`-`)
- Opções sem argumentos podem ser agrupadas após o hífen
- O primeiro argumento de opção, após uma opção, deve ser precedido por um espaço em branco. Por exemplo, `-o sfile` é válido, mas `-osfile` é ilegal.
- Os argumentos da opção não são opcionais
- Se uma opção tiver mais de um argumento, eles devem ser separados por vírgulas sem espaços, ou se espaços forem usados, a cadeia de caracteres (*string*) deve ser incluída entre aspas duplas (`"`). Por exemplo, ambos os seguintes são aceitáveis:
  - `-f past,now,next` e 
  - `-f "past now next"`
- Todas as opções devem preceder outros argumentos na linha de comando
- Um hífen duplo (`--`) pode ser usado para indicar o fim da lista de opções
- A ordem das opções é independente da ordem
- A ordem dos argumentos pode ser importante
- Um único hífen (`-`) é usado para significar entrada padrão
  

## Obtendo Ajuda em Comandos UNIX

A opção longa `--help` costuma ser encontrada em comandos tanto para Linux, Mac e Windows, e em comandos de aplicações gráficas (GUI, como `firefox --help`, `google-chrome --help`, `code --help`) como em comandos para a linha de comandos (CLI, como `cp --help`, `ln --help`, `ssh --help`). Ela exibe uma ajuda resumida de uso do comando executado com ela. Da próxima vez que se for aprender um comando novo, experimente executar: `COMANDO --help`

E veja o que ele devolve.

Exemplos comuns de uso de comandos podem ser visto com o comando `tldr` (Abreviação para *Too Long; Don't Read* -- "Longo Demais; Não Leia" em inglês). Exemplos:

- `tldr ssh`
- `tldr exit`
- `tldr whoami`

