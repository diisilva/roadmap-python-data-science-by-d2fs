# Laboratório opcional — ML por dentro

[← Guia de estudo](../../guias/ml-from-scratch.md) · [Fase 3](../../README.md#fase-3--machine-learning-clássico-semanas-1520)

Use esta pasta para produzir código autoral a partir do que você entendeu no snapshot `ML-From-Scratch`. Não copie a implementação original e não modifique o snapshot.

## Escolha

Implemente somente um algoritmo:

- regressão linear por gradiente descendente;
- regressão logística binária; ou
- árvore de decisão pequena para classificação.

## Estrutura sugerida

```text
projects/ml-from-scratch-lab/
├── README.md
├── src/
│   └── model.py
├── tests/
│   └── test_model.py
└── report.md
```

Crie os arquivos conforme avançar. Registre em `report.md` a formulação matemática, o experimento, a comparação e as limitações.

## Contrato da entrega

- API mínima com `fit(X, y)` e `predict(X)`;
- dataset sintético pequeno e semente fixa;
- teste de formato e de um resultado conhecido;
- ao menos um caso extremo, como entrada constante ou classe ausente;
- comparação com o equivalente do scikit-learn usando a mesma divisão;
- métrica adequada e diferença entre os resultados explicada;
- nenhuma leitura do conjunto de teste durante o ajuste.

## Checklist

- [ ] Consigo explicar cada etapa do algoritmo sem consultar o código original.
- [ ] Os testes falham se eu introduzir deliberadamente um erro central.
- [ ] A comparação usa os mesmos dados e protocolo nos dois modelos.
- [ ] Documentei simplificações, limites numéricos e custo computacional.
- [ ] Registrei a evidência da entrega em [`PROGRESS.md`](../../PROGRESS.md).
