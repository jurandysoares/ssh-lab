# Laço Ler-Avaliar-Exibir

O interpretador de comandos do terminal, também conhecido como *shell*, seguirá o laço Ler-Avaliar-Exibir (REPL, na sigla em inglês).

## Inglês

```mermaid
graph LR
  read[Read]
  eval[Eval]
  print[Print]

  read --> eval --> print --> read
```

## Português
```mermaid
graph LR
  read[Ler]
  eval[Avaliar]
  print[Exibir]

  read --> eval --> print --> read
```

## Referência
- [Read–eval–print loop - Wikipedia](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop)
