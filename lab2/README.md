# Laboratório 2 - Ciência de Dados Preditiva

* [Parte 1](#parte-1)
    * [Descrição](#descrição)
    * [Perguntas](#perguntas)
* [Parte 2](#parte-2)

## Parte 1
### Descrição

Nessa atividade vamos explorar dados sobre as votações que candidatos à Câmara Federal de Deputados receberam nos anos de 2006 e 2010. A nossa tarefa é usar Regressão Linear para explicar essas votações. Esses dados foram extraídos do [TSE](http://www.tse.jus.br/hotSites/pesquisas-eleitorais/index.html), pré-processados e contemplam informações sobre aproximadamente 7.300 candidatos. A descrição de cada atributo é dada abaixo:

* "sequencial_candidato": (character) id do candidato
* "nome": (character)
* "uf": (character)
* "partido": (character)
* "quantidade_doacoes": (integer)
* "quantidade_doadores": (integer) número de doadores diferentes
* "total_receita": (double) soma em R$ das doações
* "media_receita": (double) média das doações
* "recursos_de_outros_candidatos/comites": (double) quantia em R$ das doações provenientes de outros candidatos ou comite partidária
* "recursos_de_pessoas_fisicas": (double) quantia em R$ das doações provenientes de outros CPFs
* "recursos_de_pessoas_juridicas": (double) quantia em R$ das doações provenientes de outros CNPJ
* "recursos_proprios": (double) quantia em R$ das doações provenientes do próprio candidato
* "recursos_de_partido_politico": (double) quantia em R$ das doações provenientes do partido político do candidato
* "votos": (integer) variável alvo. Se refere ao número de votos na campanha de 2006 e 2010
* "quantidade_despesas": (integer)
* "quantidade_fornecedores": (integer) número de fornecedores/despesas diferentes
* "total_despesa": (double) soma em R$ das despesas de campanha
* "media_despesa": (double) média das despesas de campanha
* "cargo": (character)
* "Sexo":  (character)
* "grau": (character) grau de instrução do candidato
* "estado_civil": (character)
* "ocupacao": (character) ocupação do candidato

### Perguntas

De forma mais específica, vocês vão responder as seguintes perguntas:

1. Um modelo de regressão múltipla com todas as variáveis é plausível para explicar a variação em y (número de votos) em 2006? Mesma pergunta para 2010. 
2. Compare as regressões construídas para 2006 e 2010. Quais as diferenças/semelhanças percebidas? Algumas sugestões:
    1. Analise os plots de resíduos e verifique se há tendências nos erros para cada ano.
    2. Quais variáveis conseguem explicar melhor o número de votos? Compare essas variáveis entre os modelos. Mesma coisa para as variáveis menos explicativas.
    3. Compare os valores de R2 e RSE considerando as regressões para cada ano.
    4. Inclua outros pontos de comparação que você ache interessante.
3. Todas as variáveis são úteis para os modelos de regressão? Há variáveis redudantes? Faça análises para 2006 e 2010 separadamente. 
4. No caso de haver variáveis pouco explicativas e/ou redudantes, construa um novo modelo sem essas variáveis e o compare ao modelo com todas as variáveis (e.g. em termos de R2 e RSE). Faça isso para 2006 e 2010 separadamente. 
5. Construa agora uma regressão considerando os anos 2006 e 2010 em conjunto. Que diferenças/semelhanças você percebe em relação aos modelos individuais por ano? Veja a questão 2 para sugestões que você usar para comparação.

## Parte 2
### Descrição 

Nesta parte construiremos modelos preditivos de regressão para a predição de votação de candidatos à Câmara Federal de Deputados, As atividades esperadas para essa etapa são descritas a seguir:

### Perguntas

1. Usando todas as variáveis disponíveis, tune (usando validação cruzada):
    1. um modelo de regressão Ridge,
    2. um modelo de regressão Lasso e 
    3. um modelo KNN.

    Para os modelos de regressão linear, o parâmetro a ser tunado é o lambda (penalização dos coeficientes) e o KNN o número de vizinhos. (9 pts.)
2. Compare os três modelos em termos do erro RMSE de validação cruzada. (9 pts.)
3. Quais as variáveis mais importantes segundo o modelo de regressão Ridge e Lasso?  Variáveis foram descartadas pelo Lasso? Quais? (9 pts.)
4. Re-treine o melhor modelo (usando os melhores valores de parâmetros encontrados em todos os dados, sem usar validação cruzada). (9 pts.)
5. Use esse último modelo treinado para prever os dados de teste disponíveis [no challenge que criamos na plataforma Kaggle](https://www.kaggle.com/c/ufcg-cdp-20182) (9 pts.)

### Ideias para melhorar os resultados

* Tente criar novas variáveis a partir das variáveis existentes. Usar dados externos seria uma opção, mas no nosso caso não será possível pois para isso os dados de teste que estão conosco também teriam que ter esses novos atributos derivados de dados externos.
* Usando outros métodos de regressão. Por exemplo, SVR, Árvores de Regressão e Florestas Aleatórias.