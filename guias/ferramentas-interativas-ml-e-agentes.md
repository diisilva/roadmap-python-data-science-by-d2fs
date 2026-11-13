# Guia de estudo — sistemas de ML e analytics com agentes

[← Índice](../README.md#cockpit-das-40-aulas) · [Fonte original](https://github.com/Future-Proof-DS/interactive-ai-ml-tools)

## Papel no roadmap

As cinco ferramentas interativas de [Future Proof Data Science](https://futureproofds.com/tools) ajudam a visualizar componentes de sistemas de ML em produção e de analytics com agentes. São **externas e opcionais**: use cada uma depois do material principal da aula correspondente. Os tempos abaixo são estimativas do autor, não carga adicional obrigatória da trilha.

| Aula | Ferramenta | Tempo | Evidência curta |
|---|---|---:|---|
| 27 | [Anatomy of a Production ML System](https://futureproofds.com/tools/ml-system-map) | 20 min | Desenho do fluxo entre dados, treino, avaliação, serviço e monitoramento no seu projeto. |
| 27 | [ML Project Structure](https://futureproofds.com/tools/ml-project-structure) | 15 min | Árvore de pastas proposta para o projeto da aula 20, com uma responsabilidade por pasta. |
| 30 | [Data Drift Simulator](https://futureproofds.com/tools/ml-data-drift) | 15 min | Registro do sinal observado, da hipótese de causa e da ação de investigação. |
| 36 | [Agentic Analytics System Map](https://futureproofds.com/tools/agentic-analytics-system) | 20 min | Diagrama de uma pergunta, das ferramentas e dos controles até a resposta. |
| 37 | [Evals, Step by Step](https://futureproofds.com/tools/ai-evals) | 5 min | Dois casos de avaliação com entrada, resultado esperado e critério de aprovação. |

## Roteiro de aplicação

### Aulas 27 e 30 — Do modelo ao sistema

1. No mapa do sistema, identifique onde seu projeto prepara dados, treina, registra a versão, serve previsões e coleta sinais de produção. Marque os componentes que ainda não existem.
2. Na estrutura de projeto, compare a organização apresentada com o seu código. Separe configuração, transformação, treino, avaliação, inferência e testes conforme as responsabilidades reais do projeto; não crie pastas vazias apenas para reproduzir o exemplo.
3. No simulador de drift, escolha uma mudança observável nos dados de entrada e descreva como monitoraria essa distribuição em relação a uma referência versionada. Registre volume da amostra e período de comparação.
4. Explique qual evidência adicional seria necessária para afirmar queda de desempenho: drift nos dados, sozinho, não mede a qualidade das previsões. Proponha uma investigação antes de decidir por novo treino ou rollback.

### Aulas 36 e 37 — Do agente à avaliação

1. No mapa de analytics, trace o caminho de uma pergunta de negócio até a resposta: contexto, definição da métrica, consulta, validação do resultado e apresentação. Indique onde aplicar permissões e limites às ferramentas.
2. Crie um caso em que a pergunta é ambígua e outro em que a consulta seria inadequada. Defina quando o agente deve pedir esclarecimento ou recusar a operação.
3. Em evals, escreva pelo menos dois casos com pergunta, dados ou fontes disponíveis, resultado esperado e regra verificável. Compare o valor calculado e a consulta ou trajetória usada; uma resposta plausível pode conter um número errado.
4. Execute os casos antes e depois de uma mudança no agente. Guarde as falhas encontradas como regressões e registre a versão avaliada.

## Limites do material

As ferramentas são demonstrações didáticas no navegador. Use-as para formular hipóteses e desenhar seus próprios controles; a evidência da trilha continua sendo o código e a avaliação do seu projeto. O [repositório público do autor](https://github.com/Future-Proof-DS/interactive-ai-ml-tools) funciona como catálogo das ferramentas. Este guia resume objetivos de estudo e aponta para as páginas oficiais; nenhum código ou asset do projeto foi incorporado.
