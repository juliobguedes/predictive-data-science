# Laboratório 3 - Ciência de Dados Preditiva

## Descrição

Nessa atividade você irá usar seus conhecimentos sobre classificação para prever quais candidatos à Câmara de Deputados serão eleitos nas eleições de 2014. De forma específica faremos o seguinte:

## Perguntas

1. Há desbalanceamento das classes (isto é, uma classe tem muito mais instâncias que outra)? Em que proporção? Quais efeitos colaterais o desbalanceamento de classes pode causar no classificador? Como você poderia tratar isso? (10 pt.)
2. Treine: um modelo de KNN, regressão logística, uma árvore de decisão e um modelo de adaboost. Tune esses modelos usando validação cruzada e controle overfitting se necessário, considerando as particularidades de cada modelo.  (20 pts.)
3. Reporte precision, recall e f-measure no treino e validação. Há uma grande diferença de desempenho no treino/validação? Como você avalia os resultados? Justifique sua resposta. (10 pt.)
4. Interprete as saídas dos modelos. Quais atributos parecem ser mais importantes de acordo com cada modelo? (20 pts.)
5. Envie seus melhores modelos [à competição do Kaggle](https://www.kaggle.com/c/ufcg-cdp-20182-lab3/). Faça pelo menos uma submissão. Sugestões para melhorar o modelo: (20 pts.)
    * Experimente outros modelos (e.g. SVM, RandomForests e GradientBoosting).
    * Experimente balancear as classes,  caso estejam desbalanceadas.
    * Experimente outras estratégias de ensembles (e.g. Stacking)