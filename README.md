# Roadmap Python, Dados e IA by D2FS

Uma trilha prática de 40 semanas para sair dos fundamentos de Python e chegar à construção de soluções completas com dados, machine learning, engenharia de dados e inteligência artificial.

O foco não é concluir o maior número possível de cursos. O foco é produzir evidências de aprendizado: código autoral, testes, análises, pipelines, modelos avaliados e um projeto final de portfólio.

## Para quem é este roadmap

Este roteiro foi criado para pessoas iniciantes ou em transição de carreira que conseguem estudar de 5 a 7,5 horas por semana. Não é necessário conhecer machine learning, mas é importante saber usar arquivos e pastas no computador e estar disposto a consultar materiais em inglês.

Ao terminar a trilha essencial, a pessoa deverá conseguir:

- escrever, testar e organizar aplicações Python;
- consultar, limpar, analisar e visualizar dados;
- explicar e avaliar modelos clássicos de machine learning;
- construir um pipeline de dados reproduzível;
- transformar um modelo em uma aplicação observável;
- criar e avaliar uma aplicação com LLM, RAG ou agente;
- apresentar um projeto completo com documentação técnica.

## Como usar

- Trabalhe em somente um material principal por vez.
- Use no máximo uma segunda fonte como referência.
- Faça cinco sessões semanais de 60 a 90 minutos.
- Registre toda entrega em [PROGRESS.md](./PROGRESS.md).
- Avance somente depois de cumprir o critério de conclusão da fase.
- Use as semanas 14 e 26 para revisão, recuperação e organização do portfólio.
- Não baixe modelos ou datasets grandes antes de realmente precisar deles.

### Legenda

- **Essencial:** faz parte das 40 semanas.
- **Opcional:** aprofundamento depois da trilha ou quando houver tempo adicional.
- **Incluído:** snapshot disponível dentro deste repositório.
- **Externo:** link para a versão mantida pelo autor original.

## Trilha essencial — 40 semanas

### Fase 0 — Ambiente e ferramentas (semanas 1–2)

Competências: terminal, Git, GitHub, ambientes virtuais, instalação de dependências, depuração e testes básicos.

Material principal: [Tutorial oficial do Python](https://docs.python.org/pt-br/3/tutorial/) — externo.

Entrega: repositório com um programa de terminal, pelo menos três testes e instruções de execução.

Critério de conclusão: clonar o projeto em outra pasta, preparar o ambiente e executar aplicação e testes usando apenas o README.

### Fase 1 — Python aplicado (semanas 3–7)

Competências: tipos, coleções, funções, módulos, arquivos, exceções, orientação a objetos e consumo básico de APIs.

Material principal: tutorial oficial e exercícios autorais. O [Python-100-Days](https://github.com/jackfrued/Python-100-Days) é uma referência opcional externa e seu conteúdo principal está em chinês.

Entrega: aplicação de terminal para tarefas, despesas ou análise de CSV, com persistência e testes.

Critério de conclusão: implementar uma funcionalidade nova sem copiar uma solução e explicar as decisões do código.

### Fase 2 — Análise de dados, estatística e SQL (semanas 8–13)

Competências: NumPy, pandas, visualização, estatística descritiva, amostragem, correlação, SQL, joins e agregações.

Materiais principais:

- [PythonDataScienceHandbook](./PythonDataScienceHandbook/) — incluído.
- [Tutorial SQL do PostgreSQL](https://www.postgresql.org/docs/current/tutorial-sql.html) — externo.

Entrega: análise exploratória reproduzível com perguntas, limpeza, consultas SQL, visualizações e conclusões.

Critério de conclusão: partir dos dados brutos e gerar novamente todos os resultados sem etapas manuais ocultas.

### Revisão 1 — Fundamentos (semana 14)

- Refazer um exercício de Python sem consulta.
- Revisar o projeto de análise e remover código duplicado.
- Conferir testes, README, dependências e evidências no `PROGRESS.md`.
- Recuperar lacunas antes de começar machine learning.

### Fase 3 — Machine learning clássico (semanas 15–20)

Competências: preparação de dados, baseline, treino e validação, prevenção de vazamento, métricas, interpretação e análise de erros.

Material principal: [ML-For-Beginners](https://github.com/microsoft/ML-For-Beginners) — externo.

Entrega: projeto de classificação ou regressão comparando baseline e pelo menos dois modelos.

Critério de conclusão: justificar divisão dos dados, escolha das métricas, resultado e principais erros do modelo.

### Fase 4 — Engenharia de dados (semanas 21–25)

Competências: ingestão, modelagem, transformação, armazenamento, qualidade, orquestração e execução idempotente.

Material principal: [Data Engineering Zoomcamp](https://github.com/DataTalksClub/data-engineering-zoomcamp) — externo.

Entrega: pipeline que transforma dados brutos em uma tabela analítica e pode ser executado novamente.

Critério de conclusão: obter o mesmo resultado em uma execução limpa e documentar arquitetura, entradas, saídas e falhas esperadas.

### Revisão 2 — Dados e modelos (semana 26)

- Executar novamente os projetos das fases 2, 3 e 4.
- Corrigir dependências, caminhos absolutos e instruções incompletas.
- Escrever uma retrospectiva sobre qualidade dos dados e confiabilidade dos modelos.
- Escolher o domínio do projeto final.

### Fase 5 — Engenharia de machine learning (semanas 27–30)

Competências: organização de projeto, versionamento de dados e modelos, testes, rastreamento de experimentos, serviço de inferência e monitoramento básico.

Material principal: [Made-With-ML](./Made-With-ML/) — incluído.

Entrega: transformar o modelo da fase 3 em um pipeline testável e reproduzível.

Critério de conclusão: executar treino e avaliação por comando, validar entradas e registrar métricas e versão do modelo.

### Fase 6 — IA generativa e fundamentos de LLMs (semanas 31–34)

Competências: tokenização, embeddings, atenção, contexto, inferência, prompting, avaliação e limitações.

Materiais principais:

- [Generative AI for Beginners](https://github.com/microsoft/generative-ai-for-beginners) — externo.
- [LLMs-from-scratch](./LLMs-from-scratch/) — incluído como referência técnica.

Entrega: aplicação pequena com LLM, conjunto de casos de teste e registro de custo, latência e falhas.

Critério de conclusão: explicar como a entrada vira tokens, como o contexto é usado e onde a aplicação pode produzir respostas incorretas.

### Fase 7 — RAG e agentes (semanas 35–37)

Competências: recuperação de documentos, ferramentas, memória, estado, observabilidade, guardrails e avaliação.

Material principal: [AI Agents for Beginners](https://github.com/microsoft/ai-agents-for-beginners) — externo.

Entrega: aplicação que consulta documentos próprios ou utiliza uma ferramenta com tratamento de falhas.

Critério de conclusão: demonstrar casos de sucesso e falha, manter logs e medir a qualidade com um conjunto pequeno de avaliações.

### Fase 8 — Projeto final (semanas 38–40)

Construa um MVP que una dados, modelo e aplicação. O escopo e a rubrica estão em [projects/capstone/README.md](./projects/capstone/README.md).

Entrega mínima:

- ingestão e validação de dados;
- análise ou transformação reproduzível;
- modelo clássico ou aplicação com LLM;
- testes e avaliação mensurável;
- interface por CLI, API ou aplicação web;
- documentação de arquitetura, execução, limitações e próximos passos.

Critério de conclusão: outra pessoa consegue executar o projeto e verificar ao menos uma métrica sem orientação verbal.

## Especializações opcionais

Estes materiais não fazem parte das 40 semanas. Escolha uma área somente depois do projeto final.

| Área | Materiais sugeridos |
|---|---|
| Fundamentos amplos de IA | [AI-For-Beginners](https://github.com/microsoft/AI-For-Beginners) |
| Deep learning | [TensorFlow-Examples](https://github.com/aymericdamien/TensorFlow-Examples) |
| Prompting | [Prompt Engineering Interactive Tutorial](https://github.com/anthropics/prompt-eng-interactive-tutorial) |
| Receitas de LLM | [OpenAI Cookbook](https://github.com/openai/openai-cookbook) e [Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) |
| Aplicações e RAG | [llm-app](https://github.com/pathwaycom/llm-app) e [dive-into-llms](https://github.com/Lordog/dive-into-llms) |
| Engenharia de dados | [Data Engineer Handbook](https://github.com/DataExpert-io/data-engineer-handbook) |
| Visão computacional | [Segment Anything](https://github.com/facebookresearch/segment-anything) |
| Geração de imagens | [Stable Diffusion](https://github.com/CompVis/stable-diffusion) |
| Áudio generativo | [Bark](https://github.com/suno-ai/bark) |
| Pesquisa | [Google Research](https://github.com/google-research/google-research) |

## Requisitos técnicos

Para as fases 0–5, um computador com 8 GB de RAM é suficiente para a maioria dos exercícios pequenos. Para LLMs e multimodalidade, prefira APIs, Colab ou modelos pequenos quando não houver GPU dedicada. Sempre confira custos antes de ativar serviços em nuvem.

Preparação básica por projeto:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
```

Depois, siga o `README.md`, `requirements.txt` ou `pyproject.toml` do material. Não instale todas as dependências globalmente.

## Conteúdo incluído e manutenção

Somente três projetos com licenças identificadas são incluídos como snapshots:

- `PythonDataScienceHandbook` — código MIT e texto CC-BY-NC-ND;
- `Made-With-ML` — MIT;
- `LLMs-from-scratch` — Apache-2.0.

Os demais materiais são links externos para que o estudante use a versão mantida pelos autores. Consulte [SOURCES.md](./SOURCES.md) para commits, licenças e atribuições.

Os 20 diretórios de estudo permanecem na máquina que originou o roadmap, mas os metadados Git individuais foram removidos. Para atualizar um deles, faça um novo clone do projeto oficial. Essa informação descreve apenas o ambiente local e não afeta quem clonar o roadmap publicado.

## Licenciamento

Os arquivos originais do roadmap criados pela D2FS usam a licença MIT disponível em [LICENSE](./LICENSE). Cada snapshot de terceiro continua sujeito exclusivamente à própria licença; a licença da D2FS não altera nem substitui esses termos.

## Próxima ação

Preencha o diagnóstico inicial de [PROGRESS.md](./PROGRESS.md) e comece pela Fase 0. O primeiro objetivo é criar um projeto Python pequeno que outra pessoa consiga instalar, testar e executar.
