# flights-MLE

## Flight Delay Prediction

Este projeto tem como objetivo prever atrasos em voos utilizando técnicas de Machine Learning aplicadas a dados operacionais da aviação.

## Objetivo

Construir um modelo capaz de identificar, antes da decolagem, a probabilidade de um voo sofrer atraso, auxiliando na tomada de decisão operacional.

## Abordagem

O problema foi tratado como uma classificação binária, onde:

0 → voo sem atraso relevante
1 → voo com atraso

Foram testados diferentes modelos, com foco em performance e escalabilidade, sendo o principal:

LightGBM (Gradient Boosting)

## Pipeline

O fluxo do projeto inclui:

Pré-processamento
Tratamento de valores nulos
Encoding de variáveis categóricas (OneHotEncoder)
Normalização de variáveis numéricas
Feature Engineering
Criação de variáveis como:
rota (ORIGIN + DESTINATION)
interações entre companhia e rota
variáveis temporais (hora, mês, etc.)
Modelagem
Logistic Regression (baseline)
LightGBM (modelo principal)
Avaliação
Accuracy
Precision
Recall
F1 Score
ROC AUC

## Resultados

O modelo LightGBM apresentou melhor desempenho geral:

Melhor capacidade de identificar atrasos (recall)
Melhor equilíbrio entre precisão e cobertura (F1)
ROC AUC superior ao baseline

Além disso, foi aplicado ajuste de threshold, melhorando a performance conforme o objetivo do problema.

## Tecnologias
Python
Pandas / NumPy
Scikit-learn
LightGBM

## Observação

Este projeto foi desenvolvido com foco em aprendizado prático e construção de portfólio em Data Science / Machine Learning.

Video do projeto: https://youtu.be/qgsMZuFeqCo
