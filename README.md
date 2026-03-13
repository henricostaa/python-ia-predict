# Python IA Predict — Score de Crédito de Clientes

> Projeto de Machine Learning para classificação de score de crédito com foco em análise de dados, modelagem supervisionada e aplicação prática em contexto bancário.

## Visão Geral
Este projeto analisa dados de clientes de um banco para prever o **score de crédito** (`Good`, `Standard`, `Poor`).  
A solução foi construída em notebook, com pipeline de preparação de dados, treinamento de modelos e previsão para novos clientes.  
O objetivo é demonstrar capacidade de transformar dados em decisões de negócio com abordagem simples, explicável e orientada a resultado.

## Problema de Negócio e Impacto
Instituições financeiras precisam avaliar risco de crédito com rapidez e consistência. Neste projeto, usei atributos de perfil financeiro e comportamento de pagamento para automatizar a classificação de risco de novos clientes, reduzindo subjetividade e acelerando triagens iniciais de concessão de crédito.

## Descrição do Projeto (3–5 linhas)
A base `clientes.csv` é carregada e tratada com codificação de variáveis categóricas (`profissao`, `mix_credito`, `comportamento_pagamento`).  
Em seguida, os dados são divididos em treino e teste para comparação entre **Decision Tree** e **KNN**.  
O melhor modelo é utilizado para prever o score de clientes da base `novos_clientes.csv`.  
Além disso, o notebook traz análise de acurácia, matriz de confusão e importância de variáveis para interpretação dos resultados.

## Tecnologias Utilizadas
- **Python**
- **Pandas** (manipulação de dados)
- **Scikit-learn** (modelagem e métricas)
- **Matplotlib / Seaborn** (visualização)
- **Jupyter Notebook**

## Funcionalidades Principais
- Leitura e análise exploratória de uma base com **100.000 registros** de clientes.
- Pré-processamento com `LabelEncoder` para variáveis categóricas.
- Treinamento e comparação de dois algoritmos de classificação (Árvore de Decisão e KNN).
- Avaliação com acurácia e matriz de confusão.
- Predição do score para novos clientes com saída pronta para tomada de decisão.

## Diferenciais do Projeto
- **Comparação de modelos** em um mesmo fluxo, favorecendo decisão técnica baseada em métrica.
- **Interpretação do modelo** via importância de variáveis (foco em explicabilidade).
- **Pipeline objetivo e didático**, útil tanto para portfólio quanto para estudos de ML aplicado.
- **Aplicação realista de negócio** (risco de crédito), tema altamente relevante no mercado.

## Estrutura do Projeto
```bash
.
├── inicial.ipynb        # Notebook principal com pipeline completo
├── clientes.csv         # Base histórica com score de crédito (target)
├── novos_clientes.csv   # Base de novos clientes para predição
└── README.md            # Documentação do projeto
```

## Como Rodar Localmente
### 1) Clone o repositório
```bash
git clone https://github.com/seu-usuario/python-ia-predict.git
cd python-ia-predict
```

### 2) Crie e ative o ambiente virtual
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# .venv\Scripts\activate   # Windows
```

### 3) Instale as dependências
```bash
pip install pandas scikit-learn matplotlib seaborn jupyter
```

### 4) Execute o notebook
```bash
jupyter notebook inicial.ipynb
```

## Aprendizados Técnicos
Este projeto consolidou práticas importantes de ciência de dados aplicada:
- preparação de dados para algoritmos supervisionados;
- escolha de modelo orientada por métricas;
- interpretação de performance com matriz de confusão;
- conexão entre modelagem e impacto em decisões de negócio.

## Autor
**Henrique**  
[LinkedIn](https://www.linkedin.com/in/henriquecostadsantos/) • [GitHub](https://github.com/henricostaa)
