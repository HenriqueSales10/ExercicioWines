# Classificação de Vinhos com Scikit-Learn

## Descrição do Projeto

Este pequeno exercício possui o objetivo de comparar o desempenho de três algoritmos de classificação (Árvore de Decisão, Random Forest, e K-Nearest Neighbors) no conjunto de dados de vinhos do scikit-learn. 

## Estrutura do código

1. **Carregar e Explorar o Dataset**
   - Foi utilizado o dataset `load_wine` do scikit-learn, suas características principais foram exibidas e exploradas para entender o conteúdo e a estrutura dos dados.

2. **Pré-processamento dos Dados**
   - Dividi o conjunto de dados em treino (70%) e teste (30%) e apliquei a normalização usando `StandardScaler` para padronizar as features.

3. **Treinamento e Avaliação dos Modelos**
   - Foram treinados três modelos:
     - Decision Tree
     - Random Forest
     - K-Nearest Neighbors
   - Cada modelo foi avaliado com as métricas de acurácia, precisão, recall, F1-score e a matriz de confusão também foi gerada.

4. **Comparação**
   
i. Valores das Métricas para Cada Modelo

![image](https://github.com/user-attachments/assets/9ec62f8d-1a40-46cf-95af-e8bb8f521f96)

ii. Modelo com Melhor Acurácia

O Random Forest teve a melhor acurácia, classificando todas as instâncias corretamente com uma acurácia de 100%.

iii. Métrica Mais Relevante

A acurácia foi a métrica principal utilizada, pois todas as classes têm uma distribuição equilibrada, o que reduz a necessidade de priorizar outras métricas, como recall ou precision para classes minoritárias.
No entanto, a F1-score é uma métrica que considera tanto precisão quanto recall e confirma a robustez do modelo com um valor de 1.0 para o Random Forest.

iv. Diferença de Desempenho

O Random Forest teve uma performance significativamente melhor. Acredito que isso foi devido à sua estrutura baseada em várias árvores de decisão, o que o torna mais robusto a variações nos dados e permite capturar relações complexas melhor que um único modelo de árvore de decisão ou KNN.

# **Conclusão**

Após a verificação dos resultados, foi possível verificar que o Random Forest apresentou o melhor desempenho, atingindo uma acurácia e F1-score perfeitos para o conjunto de dados.
Acredito que a razão para o desempenho superior do Random Forest é sua capacidade de generalizar bem e reduzir o overfitting através da agregação de múltiplas árvores. Isso permitiu capturar padrões complexos no conjunto de dados.
As características dos dados, como a variabilidade e a diversidade dos valores nas 13 features, ajudam modelos complexos como Random Forest a capturar relações entre atributos que diferenciam as classes de vinho com alta precisão.
