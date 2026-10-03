# AT1 — Perceptron e KNN em Prática

Atividade avaliativa da disciplina de **Aprendizagem de Máquina**: implementação dos algoritmos Perceptron e K-Nearest Neighbors (KNN) usando apenas **NumPy**, em um único Jupyter Notebook.

**Aluno:** Carlos Eduardo Campos Takeshita

## Conteúdo

O notebook [`at1_am.ipynb`](at1_am.ipynb) está dividido em três desafios:

| Desafio | Problema | Técnica |
|---|---|---|
| 1 | Triagem de transações com risco de fraude | Perceptron com treinamento pela regra de Rosenblatt |
| 2 | Predição de risco de churn em clientes SaaS | Classificador KNN (distâncias Euclidiana e Manhattan) |
| 3 | Recomendação de servidores cloud | Similaridade espacial por distância Euclidiana |

## Resultados

**Desafio 1 — Perceptron** (pesos e viés iniciados em zero, η = 0.1)

- Convergência na época 6, com `w = [0.05, 0.1]` e `b = -0.8`
- Transação A `[2.5, 2.0]`: Transação Legítima
- Transação B `[8.0, 6.5]`: Transação Suspeita

**Desafio 2 — KNN** (K = 3)

- Cliente 1 `[4.0, 1.0]`: Baixo Risco
- Cliente 2 `[17.0, 5.0]`: Alto Risco

**Desafio 3 — Recomendação** (K = 2, demanda `[12, 28, 450]`)

1. Database Enterprise — distância 50.32
2. Medium Backend & Cache — distância 200.40

## Como executar

Requisitos: Python 3 e NumPy.

```bash
pip install numpy jupyter
jupyter notebook at1_am.ipynb
```

No Jupyter, use **Restart Kernel and Run All Cells** para executar tudo do início ao fim. O notebook também abre no VS Code (extensões Python e Jupyter) e no Google Colab.

## Estrutura

```
at1-am/
├── at1_am.ipynb   # notebook com os três desafios
└── README.md
```
