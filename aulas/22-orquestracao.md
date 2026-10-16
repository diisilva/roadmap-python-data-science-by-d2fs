# Aula 22 — Orquestração

[← Aula 21](./21-docker-postgresql-e-terraform.md) · [Índice](../README.md#cockpit-das-40-aulas) · [Aula 23 →](./23-data-warehouse.md)

## Objetivo

Transformar etapas soltas em um workflow com dependências, parâmetros, retentativas, logs e agendamento.

## Estude nesta ordem

1. [Zoomcamp: workflow orchestration](https://github.com/DataTalksClub/data-engineering-zoomcamp/tree/main/02-workflow-orchestration)
2. [Conceitos de flow no Kestra](https://kestra.io/docs/workflow-components/flow)

## Prática e entrega

Orquestre download, validação, carga e transformação. Provoque uma falha e confirme logs, retry e retomada segura.

## Avance quando

- [ ] Dependências e parâmetros estão explícitos.
- [ ] Uma falha pode ser diagnosticada e reexecutada sem corromper o destino.

