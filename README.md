# DataPreparation

Projeto de preparação de dados para classificação de personalidade (Introvertido vs Extrovertido).

## Descrição
Este repositório contém o pipeline de preparação de dados para um conjunto de dados gerado a partir de um modelo de deep learning treinado no conjunto de dados Extrovert vs Introvert Behavior. O objetivo principal é limpar, transformar e balancear os dados antes da aplicação de modelos de machine learning.

## Fonte dos dados
Os dados foram obtidos em:

- https://www.kaggle.com/competitions/playground-series-s5e7/data

O dataset inclui arquivos de treino e teste e foi gerado a partir de um modelo de deep learning, com distribuições de features próximas, mas não idênticas, ao dataset original.

## Conteúdo do projeto
- `Introvert vs. Extrovert/data_preparation_pipeline_Int_Ext.ipynb` - notebook com o processo de preparação dos dados.
- `train.csv` e `test.csv` - dados utilizados para análise e pré-processamento.
- `notebooks/` - notebooks adicionais do projeto.
- `tests/` - testes automatizados.

## Etapas de preparação de dados
O notebook realiza as seguintes etapas principais:

1. Carregamento do dataset.
2. Verificação de tipos, valores nulos e duplicatas.
3. Limpeza e preenchimento de valores faltantes.
4. Remoção de colunas irrelevantes (`id`).
5. Codificação de variáveis categóricas.
6. Seleção de features com `SelectKBest`.
7. Divisão em treino e teste.
8. Balanceamento das classes com `SMOTE`.

## Uso
1. Abra o notebook `Introvert vs. Extrovert/data_preparation_pipeline_Int_Ext.ipynb`.
2. Execute as células na ordem para reproduzir o pré-processamento.
3. Utilize os dados preparados para treinar modelos de machine learning.

## Objetivo
Preparar os dados de forma robusta para que possam ser utilizados em tarefas de classificação de personalidade, mantendo a qualidade do conjunto de dados e reduzindo vieses antes do treinamento de modelos.

