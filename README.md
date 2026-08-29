# .github — padrões da organização

Este repositório guarda os **arquivos de comunidade padrão** do Brasil Data Hub.
O que está aqui vale para **todos os repositórios da organização** que não
tiverem o seu próprio equivalente.

É público por exigência do GitHub: defaults de organização só são herdados a
partir de um repositório `.github` público, mesmo quando todos os repositórios
que os consomem são privados.

## O que ele publica

| Caminho | Efeito |
|---|---|
| [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE) | Os sete formulários de Issue, um por Issue Type |
| [`.github/ISSUE_TEMPLATE/config.yml`](.github/ISSUE_TEMPLATE/config.yml) | Links de apoio no seletor de template |

**Um repositório com `ISSUE_TEMPLATE` próprio ignora estes defaults por
inteiro** — não existe mesclagem. Por isso os formulários vivem só aqui.

## O modelo por trás disto

Os formulários são a porta de entrada de um modelo maior: sete Issue Types,
sete estágios de ciclo de vida e a regra de que **uma Issue aberta não é trabalho
aprovado**. A fonte de verdade é o repositório `docs`:

- **Modelo** — taxonomia, lifecycle, metadados, hierarquia e views do Project:
  [`governance/WORK-MANAGEMENT.md`](https://github.com/BrasilDataHub/docs/blob/main/governance/WORK-MANAGEMENT.md)
- **Protocolo para agentes** — o que consultar, quando é permitido executar:
  [`engineering/AGENT-WORK-PROTOCOL.md`](https://github.com/BrasilDataHub/docs/blob/main/engineering/AGENT-WORK-PROTOCOL.md)

Alterou um formulário aqui? Confira se o modelo continua descrito corretamente lá,
no mesmo trabalho.

## Reaproveitar em outra organização

Este repositório é a metade versionável de um padrão desenhado para ser copiado.
A outra metade são os Issue Types e os Issue Fields, provisionados por
`docs/scripts/work-setup.sh`, que aceita `BDH_ORG` e `BDH_PRODUCTS`. Copie este
repositório, rode o script e ajuste os valores de `Product`.
