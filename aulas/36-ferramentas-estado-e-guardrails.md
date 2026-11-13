# Aula 36 — Ferramentas, estado e guardrails

[← Aula 35](./35-recuperacao-e-respostas-fundamentadas.md) · [Índice](../README.md#cockpit-das-40-aulas) · [Aula 37 →](./37-agentes-e-avaliacao.md)

## Objetivo

Criar um agente simples que escolhe ferramentas, mantém somente o estado necessário e aplica limites antes de ações sensíveis.

## Estude nesta ordem

1. [Introdução a agentes](https://github.com/microsoft/ai-agents-for-beginners/tree/main/01-intro-to-ai-agents)
2. [Uso de ferramentas](https://github.com/microsoft/ai-agents-for-beginners/tree/main/04-tool-use)
3. [Context engineering](https://github.com/microsoft/ai-agents-for-beginners/tree/main/12-context-engineering)
4. [Agentes confiáveis](https://github.com/microsoft/ai-agents-for-beginners/tree/main/06-building-trustworthy-agents)

## Exploração opcional

Use o [Agentic Analytics System Map](https://futureproofds.com/tools/agentic-analytics-system) para traçar uma pergunta de negócio até a resposta e localizar os controles de acesso, validação e limites das ferramentas. Siga o [roteiro de aplicação](../guias/ferramentas-interativas-ml-e-agentes.md).

## Prática e entrega

Implemente duas ferramentas somente leitura, schema estrito, timeout, limite de passos e confirmação simulada para uma ação de maior risco.

## Avance quando

- [ ] Entradas e saídas das ferramentas são validadas.
- [ ] Loop, timeout, erro e tentativa de instrução maliciosa têm tratamento.

