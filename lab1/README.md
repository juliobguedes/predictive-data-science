# Laboratório 1 - Ciência de Dados Preditiva

* [Descrição](#descrição)
* [Parte 1](#parte-1)
    * [Nossas Perguntas](#nossas-perguntas)
* [Parte 2](#parte-2)
    * [Suas Perguntas](#suas-perguntas)

## Descrição

Para os labs de análise exploratória você usará dados sobre a despesa de deputados federais da legisLatura atual com a atividade parlamentar. A CEAP (cota para o exercício da atividade parlamentar) é uma cota única mensal destinada a custear os gastos dos deputados exclusivamente vinculados ao exercício da atividade parlamentar. Exemplos de despesa desse tipo são: passagens aéreas, telefonia, serviços postais, manutenção de escritórios de apoio à atividade parlamentar, assinatura de publicações, fornecimento de alimentação ao parlamentar, hospedagem, outras despesas com locomoção, contemplando locação ou fretamento de aeronaves, veículos automotores e embarcações, serviços de táxi, pedágio e estacionamento e passagens terrestres. Mais informações [neste link](http://www2.camara.leg.br/transparencia/acesso-a-informacao/copy_of_perguntas-frequentes/cota-para-o-exercicio-da-atividade-parlamentar). Os dados foram coletados do site de transparência da Câmara, tratados, e podem ser baixados [neste link](https://canvas.instructure.com/courses/1402758/files/67618888/download?verifier=ibyou5PYo9aaFgRaefc0keYkHhkQ2EqIArdmI1bq&wrap=1). Uma breve descrição dos dados se encontra abaixo:

* nomeParlamentar: Nome adotado pelo Parlamentar ao tomar posse do seu mandato.
* idCadastro: Número que identifica unicamente um deputado federal na CD.
* sgUF: No contexto da cota CEAP, representa a unidade da federação pela qual o deputado foi eleito e é utilizada para definir o valor da cota a que o deputado tem.
* sgPartido: Sigla do partido do parlamentar.
* tipoDespesa: O seu conteúdo é a descrição do Tipo de Despesa relativo à despesa em questão.
* especDespesa: Representa a descrição  especificação mais detalhada de um referido Tipo de Despesa.
* fornecedor: O conteúdo deste dado representa o nome do fornecedor do produto ou serviço presente no documento fiscal
* CNPJCPF: O conteúdo deste dado representa o CNPJ ou o CPF do emitente do documento fiscal, quando se tratar do uso da cota em razão do reembolso despesas comprovadas pela emissão de documentos fiscais.
* tipoDocumento: Este dado representa o tipo de documento do fiscal – 0 (Zero), para Nota Fiscal; 1 (um), para Recibo; e 2, para Despesa no Exterior.
* dataEmissao: O conteúdo deste dado é a data de emissão do documento fiscal ou a data do documento que tenha dado causa à despesa.
* valorDocumento: O seu conteúdo é o valor de face do documento fiscal ou o valor do documento que deu causa à despesa. Quando se tratar de bilhete aéreo, esse valor poderá ser negativo, significando que o referido bilhete é um bilhete de compensação, pois compensa um outro bilhete emitido e não utilizado pelo deputado (idem para o dado vlrLiquido abaixo).
* valorGlosa: O seu conteúdo representa o valor da glosa do documento fiscal que incidirá sobre o Valor do Documento, ou o valor da glosa do documento que deu causa à despesa.
* valorLiquido: O seu conteúdo representa o valor líquido do documento fiscal ou do documento que deu causa à despesa e será calculado pela diferença entre o Valor do Documento e o Valor da Glosa. É este valor que será debitado da cota do deputado. Caso o débito seja do Tipo Telefonia e o valor seja igual a zero, significa que a despesa foi franqueada.

## Parte 1
### Nossas perguntas:

Nessa tarefa você deve usar as técnicas de análise descritiva e visualização que apresentamos na aula sobre análise exploratória para responder as seguintes perguntas:

1. Quais são os deputados que gastaram mais dinheiro da CEAP? Quais são os mais econômicos? (7,5 pts)
2. Quais os estados cujos deputados gastam mais no exterior? Quais os estados cujos deputados gastam menos no exterior? (7,5 pts)
3. Quais os partidos cujos parlamentares mais usam CEAP no estado da Paraíba? Quais são os que menos usam? Mesmas perguntas considerando valores em R$. (7,5 pts)
4. Quais os deputados que mais ultrapassam o limite de CEAP do seu estado? Os dados com os limites de CEAP por estado estão disponíveis [neste link](https://canvas.instructure.com/courses/1402758/files/67618889/download?verifier=vfi4jwcg26IVtelxRY7Sm5RnhrAuKcNrOrw2Yt6Y). (7,5 pts)
5. Quais estados cujos parlamentares gastam mais com passagens aéreas? (7,5 pts)
6. Escolha três partidos e responda: Quais são os tipos de despesa mais utilizados no uso da CEAP pelos deputados desses partidos? Mesma pergunta considerando valores em R$. (7,5 pts)

## Parte 2
### Suas perguntas: 

* Escolha e descreva 2 perguntas que na sua opinião são relevantes, não são óbvias e que você gostaria de ver respondidas a partir dos dados. Para cada uma escreva uma frase curta que documenta qual você acha que será a resposta.  
* Construa o relatório final deste problema respondendo-as com estatística e visualizações.
* Inclua no seu relatório também qualquer parte do panorama geral que você criou na parte 2 deste problema que seja necessário para o leitor entender seu relatório.
