# Guia de estudo — ML-From-Scratch

[← Índice](../README.md#fase-3--machine-learning-clássico-semanas-1520) · [Snapshot](../ML-From-Scratch/) · [Laboratório](../projects/ml-from-scratch-lab/README.md)

## Papel no roadmap

O `ML-From-Scratch` é uma referência complementar para enxergar operações que bibliotecas como scikit-learn encapsulam: inicialização de parâmetros, função de perda, gradientes, critérios de divisão e agregação de previsões.

Ele não substitui o material principal da Fase 3. Use scikit-learn para construir o projeto avaliado e o snapshot para estudar uma implementação pequena, questioná-la e produzir uma versão autoral testada.

## Escopo recomendado

Não tente estudar todos os algoritmos do repositório. Complete estes quatro blocos em sessões de 60 a 90 minutos:

| Aula | Leia no snapshot | Evidência mínima |
|---|---|---|
| 16 — Regressão | `regression.py` e o exemplo linear | Derivação curta do erro e teste de `fit`/`predict` |
| 17 — Classificação | `logistic_regression.py` e o exemplo logístico | Cálculo documentado de escore, sigmoide e classe |
| 18 — Validação | utilitários de divisão e métricas | Auditoria de limitações e comparação com scikit-learn |
| 19 — Interpretação | `decision_tree.py` e `random_forest.py` | Traçado de uma previsão da raiz à folha |
| 20 — Projeto | um algoritmo escolhido | Implementação autoral comparada e testada |

### Aula 16 — Regressão por dentro

1. Leia [`supervised_learning/regression.py`](../ML-From-Scratch/mlfromscratch/supervised_learning/regression.py), concentrando-se em `Regression.fit`, `LinearRegression.fit` e `predict`.
2. Execute ou percorra [`examples/linear_regression.py`](../ML-From-Scratch/mlfromscratch/examples/linear_regression.py).
3. Explique por que a coluna de uns representa o intercepto e como o gradiente altera cada peso.
4. Implemente uma regressão linear mínima sem copiar o arquivo e compare coeficientes e MAE com scikit-learn.

### Aula 17 — Classificação por dentro

1. Leia [`supervised_learning/logistic_regression.py`](../ML-From-Scratch/mlfromscratch/supervised_learning/logistic_regression.py) e a implementação de [`Sigmoid`](../ML-From-Scratch/mlfromscratch/deep_learning/activation_functions.py).
2. Percorra [`examples/logistic_regression.py`](../ML-From-Scratch/mlfromscratch/examples/logistic_regression.py).
3. Para três exemplos pequenos, registre o escore linear, a probabilidade e a classe após o limiar.
4. Compare sua versão com scikit-learn usando a mesma divisão dos dados e discuta diferenças de intercepto, regularização e convergência.

### Aula 18 — Validação é mais que código

1. Leia `train_test_split` em [`utils/data_manipulation.py`](../ML-From-Scratch/mlfromscratch/utils/data_manipulation.py) e as métricas em [`utils/data_operation.py`](../ML-From-Scratch/mlfromscratch/utils/data_operation.py).
2. Liste o que essas funções resolvem e o que não resolvem: estratificação, grupos, ordem temporal, validação das entradas e casos extremos.
3. Escreva testes que exponham pelo menos dois limites encontrados.
4. Mantenha o protocolo da [aula 18](../aulas/18-validacao-e-metricas.md) como fonte de verdade para avaliação.

### Aula 19 — Árvores e florestas por dentro

1. Leia `_build_tree` e `predict_value` em [`supervised_learning/decision_tree.py`](../ML-From-Scratch/mlfromscratch/supervised_learning/decision_tree.py).
2. Observe como [`supervised_learning/random_forest.py`](../ML-From-Scratch/mlfromscratch/supervised_learning/random_forest.py) cria diversidade entre árvores e combina previsões.
3. Com um dataset minúsculo, desenhe a raiz, os ramos e as folhas; depois percorra manualmente uma previsão.
4. Relacione profundidade, número mínimo de amostras e variância do modelo, sem tratar importância como causalidade.

### Aula 20 — Auditoria e comparação final

Escolha regressão linear, regressão logística ou árvore de decisão e faça o [laboratório](../projects/ml-from-scratch-lab/README.md). A entrega deve conter código autoral, testes de casos normais e extremos, comparação com scikit-learn e uma seção de limitações.

## Como usar o snapshot com segurança

O snapshot reproduz o commit `a2806c6732ee`, de 18 de outubro de 2019, e preserva a licença MIT original. Seu `requirements.txt` não fixa versões e inclui dependências e APIs antigas. Portanto:

- trate o código como material de leitura e experimentação;
- não execute `setup.py install` nem instale o `requirements.txt` inteiro no ambiente do roadmap;
- crie um ambiente virtual descartável e instale somente o necessário para o exemplo escolhido;
- prefira datasets sintéticos pequenos e NumPy para a reimplementação;
- não edite o snapshot: escreva sua solução em `projects/ml-from-scratch-lab/`;
- confirme resultados contra uma implementação mantida, como scikit-learn.

O objetivo não é obter uma biblioteca própria pronta para produção. É conseguir explicar o algoritmo, reconhecer simplificações didáticas e provar o entendimento com testes.
