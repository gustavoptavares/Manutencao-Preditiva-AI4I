# Entendendo as falhas de máquinas através da manutenção preditiva

## Visão Geral

Neste projeto, vamos analisar os dados disponíveis, no conjunto de dados de manutenção preditiva AI4I 2020, que reflete dados reais de manutenção preditiva encontrados na indústria. 

Você pode conferir o dataset e o projeto na íntegra clicando abaixo:

Link dataset: https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset

Link projeto: https://github.com/gustavoptavares/Manutencao-Preditiva-AI4I/blob/main/Manuten%C3%A7%C3%A3o_Preditiva_AI4I.ipynb

## Problema e Solução

Vamos analisar os dados conjunto de dados de manutenção preditiva AI4I 2020, para entender as falhas da máquina que consiste em cinco modos de falha independentes. Com um conjunto de dados consiste em 10.000 dados armazenados como linhas com 14 colunas, vamos entender, no detalhe, aspectos das falhas da máquina, como:

• Os tipos de falhas e as suas variáveis.

• Previsão do status de falha da máquina.

## O Processo

O primeiro passo do projeto foi adquirir os dados. Utilizamos os dados do portal UCI Machine Learning Repository, carregando-o no Google Colab, para a exploração e análise dos dados utilizando a linguagem de programação Python e suas bibliotecas, como Pandas, Matplotlib e Scikit-Learn. Foi feita análise exploratória, visualização dos dados, e através do modelo de machine learning de classificação, utilizando o algortimo de regressão logística.

## Resultados

O modelo de regressão logística alcançou os seguintes resultados:

Acurácia no conjunto de treino: 99.91%

Acurácia no conjunto de teste: 99.9%

Matriz de Confusão: 1932 previsões verdadeiro negativo (TN), 66 verdadeiro positivo (TP), 2 falso negativo (FN) e 0 falso positivo (FP).

Precisão: 1.0 (Isso significa que quando o modelo prevê uma falha, ele está correto 100% das vezes.)

Recall: 0.9706 (Isso significa que o modelo identifica 97.06% das falhas reais.)

F1-score**: 0.9851 (Média harmônica de precisão e recall.)

## Conclusões

O modelo de regressão logística construído tem um desempenho muito bom na previsão de falhas de máquina, com alta precisão e recall.

Indicadores de falha, como HDF, PWF e TWF, são os preditores mais significativos de falhas na máquina.

Outras variáveis, como desgaste da ferramenta e velocidade de rotação, também desempenham um papel importante na previsão.

O desequilíbrio de classes foi considerado ao dividir os dados em conjuntos de treino e teste usando a estratificação.

Pode ser benéfico explorar técnicas de reamostragem ou outros algoritmos de classificação para verificar se o desempenho pode ser ainda melhorado ou se os resultados se mantêm consistentes.
