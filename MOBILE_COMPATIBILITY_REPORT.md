# Aurora Pet Mobile Version — Relatório de compatibilidade

## Resultado

Foi criada/reaproveitada no PC a cópia independente:

`C:\Users\samuk\OneDrive\Documentos\AuroraPetMobileVersion`

O nome interno do projeto foi configurado como **Aurora Pet Mobile Version**, com versão `0.1-mobile` e cena inicial `res://scenes/mobile_main.tscn`.

## Compatibilidade PC × GitHub

O projeto local do PC e o repositório `https://github.com/Samukax7/aurorapet.git` estavam no mesmo commit:

`020ae933c659b49847f0f931c6157bf0d9dfefec`

Os hashes SHA-256 dos arquivos críticos foram iguais nos dois lados, incluindo `project.godot`, `export_presets.cfg`, `main.tscn`, `console_frame.tscn`, `deepworld.tscn`, `mobile_main.tscn`, `mobile_main.gd`, `mobile_touch_controls.gd`, `battle_stage.tscn`, `batalha_de_exploracao.tscn` e seus controladores principais.

## Configuração da cópia mobile

| Item | Projeto principal | Cópia mobile |
|---|---|---|
| Nome | AuroraPet V 0.1 | Aurora Pet Mobile Version |
| Versão | 0.1 | 0.1-mobile |
| Cena inicial | `scenes/main.tscn` | `scenes/mobile_main.tscn` |
| Preset | Web V 0.1 | Web Mobile V 0.1 |
| Repositório Git local | Principal | Removido para manter independência |

A nova cópia mantém a lógica, as cenas, o pet modular, o Deepworld, a batalha, os minigames e a progressão. A diferença de entrada é a casca mobile com controles touch, definida em `mobile_main.tscn` e `mobile_touch_controls.gd`.

## Validação

A cópia foi executada no Godot 4.7.1 Win64 em modo headless. A primeira execução encontrou cache `.godot` inconsistente, herdado de uma cópia anterior. O cache foi removido, a importação dos assets foi concluída e a execução final não apresentou `ERROR` nem `SCRIPT ERROR`.

O projeto principal permaneceu intacto: seu nome continua `AuroraPet V 0.1`, a cena inicial continua `res://scenes/main.tscn`, e o arquivo temporário utilizado para transferir a configuração foi removido.

## Observação sobre plugins

A cópia mobile mantém os plugins locais disponíveis para prototipagem no Godot, mas eles não são necessários para executar o jogo. O clone atual do GitHub ainda contém diretórios de plugins, apesar da regra anterior do projeto indicar que eles deveriam ficar somente no PC. Essa divergência foi registrada, mas não foi alterada nesta tarefa.
