# Aula 30 — Monitoramento e release

[← Aula 29](./29-inferencia-api-e-testes.md) · [Índice](../README.md#cockpit-das-40-aulas) · [Aula 31 →](./31-tokens-embeddings-e-atencao.md)

## Objetivo

Definir um release pequeno e observável, com indicadores, limites, resposta a falhas e rollback.

## Estude nesta ordem

1. [Deploy do Made With ML](../Made-With-ML/deploy/)
2. [Utilitários do projeto](../Made-With-ML/docs/madewithml/utils.md)
3. [Google Rules of ML](https://developers.google.com/machine-learning/guides/rules-of-ml)

## Exploração opcional

Percorra o [Data Drift Simulator](https://futureproofds.com/tools/ml-data-drift) e aplique o [roteiro do guia](../guias/ferramentas-interativas-ml-e-agentes.md) ao seu projeto. Diferencie alteração na distribuição dos dados de queda de desempenho do modelo e documente qual evidência levaria a investigar, retreinar ou fazer rollback.

## Prática e entrega

Defina métricas de serviço, dados e modelo; simule dado inválido ou latência alta; registre alerta, diagnóstico, mitigação e rollback.

## Avance quando

- [ ] Cada indicador tem limite e ação associada.
- [ ] A versão em produção e o caminho de rollback são identificáveis.

