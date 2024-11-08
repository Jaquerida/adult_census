# Projeto de Machine Learning - Santander Coders 2024

Este projeto foi criado como parte do módulo **Machine Learning I** do curso Santander Coders 2024. O objetivo do projeto é treinar e avaliar modelos de machine learning para prever se uma pessoa ganha mais de $50K por ano, usando dados demográficos.

## Sobre o Dataset

Os dados foram extraídos do [banco de dados do censo de 1994](https://archive.ics.uci.edu/ml/datasets/Census+Income) por Ronny Kohavi e Barry Becker (Data Mining and Visualization, Silicon Graphics). Esse dataset também está disponível no [Kaggle](https://www.kaggle.com/datasets/uciml/adult-census-income/data). Foi selecionado um conjunto de registros limpos com as seguintes condições: ((AGE>16) && (AGI>100) && (AFNLWGT>1) && (HRSWK>0)). A tarefa de predição é determinar se uma pessoa ganha mais de $50K por ano.

### Descrição do atributo `fnlwgt` (peso final)

Os pesos nos arquivos da Pesquisa de População Atual (CPS) são ajustados para estimativas independentes da população civil não institucional dos EUA. Estes são preparados mensalmente pela Divisão de População do Census Bureau. Utilizamos três conjuntos de controles:

1. Uma estimativa de célula única da população de 16+ para cada estado.
2. Controles para Origem Hispânica por idade e sexo.
3. Controles por Raça, idade e sexo.

Utilizamos todos os três conjuntos de controles no programa de ponderação e aplicamos o "ajuste" através deles 6 vezes para garantir que todos os controles fossem considerados. A estimativa se refere a totais de população derivados do CPS por meio de "contagens ponderadas" de quaisquer características socioeconômicas especificadas da população. Pessoas com características demográficas semelhantes devem ter pesos semelhantes. Importante observar que o CPS é na verdade uma coleção de 51 amostras estaduais, cada uma com sua própria probabilidade de seleção, e a declaração aplica-se apenas dentro do estado.

### Artigos Relevantes

Ron Kohavi, ["Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid"](http://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf), Proceedings of the Second International Conference on Knowledge Discovery and Data Mining, 1996.
