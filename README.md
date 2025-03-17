# Análise e Classificação da Qualidade do Sono

## Descrição do Projeto

Este repositório contém códigos e notebooks utilizados para a análise e classificação da qualidade do sono, abrangendo desde o pré-processamento dos dados até o treinamento de modelos de machine learning para a predição da qualidade do sono.

## Estrutura do Repositório

1. Pre_processamento.ipynb

Este notebook implementa o modelo de Cole-Kripke como uma etapa inicial para a identificação dos períodos de sono e vigília. As principais etapas incluem:

* Identificação e segmentação dos períodos de sono e vigília;

* Desenvolvimento das métricas de sono com base na classificação obtida;

* Geração de hipnogramas para visualização das fases do sono;

* Exportação dos dados processados para um arquivo .csv, que será utilizado nas próximas etapas para a classificação da qualidade do sono.

2. RFE_Selecao_Metricas.ipynb

Neste notebook, realizamos a seleção das 9 métricas de sono mais relevantes para a classificação da qualidade do sono. Utilizamos a técnica Recursive Feature Elimination (RFE) para escolher as melhores variáveis com base em sua importância para a classificação.

3. Treinamento_Balanceamento_Resultados.ipynb

Este notebook é dedicado ao treinamento de uma rede neural para a classificação da qualidade do sono, utilizando o método Leave-One-Subject-Out (LOSO). Testamos o treinamento tanto com quanto sem a aplicação do SMOTE (Synthetic Minority Over-sampling Technique) para balanceamento dos dados.

As principais etapas incluem:

* Treinamento da rede neural;

* Avaliação dos resultados por meio das curvas ROC e matriz de confusão;

* Implementação dos classificadores utilizados para a predição da qualidade do sono.
