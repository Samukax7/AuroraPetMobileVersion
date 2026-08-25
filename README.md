# Aurora Pet Mobile Version

Esta é a cópia independente mobile do **AuroraPet**, um V-Pet cósmico em pixel art desenvolvido em Godot 4.7. O projeto mantém a mesma lógica de gameplay, pet modular, Deepworld, progressão, minigames e batalha da versão principal, mas inicia por uma casca própria para telas touch.

## Execução

Abra `project.godot` no Godot 4.7 ou superior e execute o projeto. A cena inicial configurada é `scenes/mobile_main.tscn`.

Para testar a versão desktop original, use o repositório principal e a cena `scenes/main.tscn`. Esta cópia possui configuração própria e não deve ser usada para substituir o projeto principal.

## Estrutura mobile

`mobile_main.tscn` instancia o `console_frame.tscn` como base lógica, remove a moldura física do console e adiciona `mobile_touch_controls.gd`. Os controles touch encaminham D-pad, VERDE, ROSA e AMARELO para os mesmos handlers usados pelos controles físicos e pelo teclado.

A cascata compartilhada permanece:

```text
mobile_main.tscn
└── Console Base [console_frame.tscn]
    └── ScreenContent
        ├── Deepworld [deepworld.tscn]
        │   └── Pet [pet.tscn]
        ├── PetUI [pet_ui.tscn]
        ├── Quarto Cósmico
        ├── Minigames
        └── Batalha de Exploração
```

## Preset de exportação

O preset `Web Mobile V 0.1` usa orientação horizontal, canvas lógico de 1080×650, tela cheia e controles touch. O preset `Web V 0.1` continua disponível para a versão desktop, mas a cena inicial desta cópia é exclusivamente `mobile_main.tscn`.

## Estado do protótipo

A versão é um protótipo em desenvolvimento. Algumas telas, textos, sons, balanceamento e posições ainda serão refinados durante a prototipagem mobile. A moldura, os plugins de edição e os caches gerados não fazem parte da lógica essencial de execução.

## Documentação

O relatório de compatibilidade entre o PC, o projeto principal e o GitHub está em `MOBILE_COMPATIBILITY_REPORT.md`. Os documentos de design permanecem disponíveis em `docs/design/`.
