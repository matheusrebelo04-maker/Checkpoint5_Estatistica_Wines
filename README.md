# Checkpoint 5 - Dataset WINES

Trabalho de análise estatística e agrupamento do dataset de vinhos `wine-clustering.csv` (178 vinhos e 13 variáveis químicas).

O notebook `Checkpoint5_Estatistica_Wines.ipynb` tem duas partes.

Na primeira, analisei o teor alcoólico (`Alcohol`) e o ácido málico (`Malic_Acid`): tabela de frequências, histograma, medidas descritivas (média, mediana, moda, variância, desvio padrão e quartis) e probabilidades calculadas com os dados e com a distribuição normal. O teor alcoólico tem média próxima de 13 e distribuição bem simétrica. O ácido málico tem média de 2,34, maior que a mediana, com cauda para a direita.

Na segunda, usei K-means para agrupar os vinhos. Antes disso padronizei as variáveis e conferi que não havia coluna de classe nem valores nulos. O Elbow e o Silhouette Score apontaram K = 3, com grupos de 65, 51 e 62 vinhos. Depois comparei os grupos pelas médias, principalmente álcool e ácido málico, e usei PCA só para desenhar os clusters em duas dimensões.

## Para rodar

Python 3.12 ou 3.13, com as bibliotecas:

pip install pandas numpy matplotlib scipy scikit-learn jupyter


O `wine-clustering.csv` precisa estar na mesma pasta do notebook. Depois é só executar todas as células. As saídas e os gráficos também já estão salvos no notebook.
