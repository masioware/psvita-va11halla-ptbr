# VA-11 Hall-A para PSVita em PT-BR

- [VA-11 Hall-A para PSVita em PT-BR](#va-11-hall-a-para-psvita-em-pt-br)
  - [Créditos para a tradução](#créditos-para-a-tradução)
  - [Dados da versão utilizada para tradução](#dados-da-versão-utilizada-para-tradução)
  - [Instalação manual](#instalação-manual)
  - [Arquivos utilitários](#arquivos-utilitários)
  - [Ferramentas úteis](#ferramentas-úteis)
  - [Debugging](#debugging)

## Créditos para a tradução

Este é um port para o PSVita da tradução PT-BR feita pelo **Project Nominono**.

- [Discord Project Nominono](https://discord.com/invite/nQPGQ6E)
- [Grupo da Steam](https://steamcommunity.com/groups/VA11BR)

## Dados da versão utilizada para tradução

- **Name**: VA-11 HALL-A: Cyberpunk Bartender Action
- **ID**: EP0995-PCSB01166_00
- **Region**: EU
- **Version**: 1.02
- **Min Firmware**: 3.67

## Instalação manual

Para realizar a instalação manualmente em um **PSVita / Emulador** é importante localizar a pasta do jogo, normalmente se encontra no diretório `/ux0/app/PCSB01166/games` e fazer a
substituição dos arquivos contidos no diretório `/src`.

## Arquivos utilitários

Estes arquivos são úteis para o desenvolvimento, porém não podem ser encontrados em meio aos aquivos no jogo para o PSVita, estes arquivos podem ser encontrados do diretório `/utils`.

> Arquivos exportados do `data.win` da versão Steam, foram obtidos com o _UndertaleModTool_.

| File                                                                   | Origin                        | Utilization |
| ---------------------------------------------------------------------- | ----------------------------- | ----------- |
| [dialogfont.png](/utils/fonts/dialogfont/dialogfont.png)               | `data.win` from Steam Version | Font Design |
| [glyphs_dialogfont.csv](/utils/fonts/dialogfont/glyphs_dialogfont.csv) | `data.win` from Steam Version | Font Config |

## Ferramentas úteis

- Emulador de PSVita: [Vita3k](https://vita3k.org/)
- Compilação e descompilação para o Game Maker Engine: [UndertaleModTool](https://github.com/UnderminersTeam/UndertaleModTool)

## Debugging

Para facilitar o desenvolvimento e o processo de depuração, é possível gerar logs utilizando a função `show_debug_message`.

```gml
  // code example:
  show_debug_message("debugging decompiled game...")
```

Conseguimos visualizar o output no terminal que abre junto à execução do Vita3k:

```log
[15:41:36.570] |T| [write_file]: \*\*\* TTY: debugging decompiled game...
```
