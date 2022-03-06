# Editores

No Linux, vários editores de texto para linha de comando são disponíveis.

Os mais famosos são:

- [micro](editores/micro.md)
- [nano](editores/nano.md)
- [vim](editores/vim.md)

A decisão de utilizar um ou outro dependerá de questões como:

- Facilidade
- Coloração de sintaxe
- Disponibilidade de extensões
- Programabilidade
- Integração com o terminal
- Dentre outras opções

Para abrir um arquivo com o editor, execute:

    EDITOR {{arquivo}}

Ou:

    EDITOR {{/caminho/para/arquivo}}

Onde:
- `EDITOR` é um dos editores listados acima e
- `{{arquivo}}` é o nome de um arquivo que se encontra no diretório atual e
- `{{/caminho/para/arquivo}}` é o caminho, absoluto ou relativo, para um arquivo (Ver [PATH](conceitos/path.md))