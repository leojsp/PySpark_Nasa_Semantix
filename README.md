# PySpark_Nasa_Semantix - 
  Consultas:   - https://techvidvan.com/tutorials/
               - http://spark.apache.org/docs/latest/rdd-programming-guide.html#transformations\n
               - https://data-flair.training/blogs/spark-tutorials-home/
               
               Base de dados
                - ftp://ita.ee.lbl.gov/traces/NASA_access_log_Jul95.gz
                - ftp://ita.ee.lbl.gov/traces/NASA_access_log_Aug95.gz

- Qual o objetivo do comando cache em Spark?
R: Ao realizar ações, são gerados processos de computação de dados, mas podemos persistir os dados em CACHE para ser usado em outras ações,
sem a necessidade de novos processamentos, tendo assim um ganho de performance.

- O mesmo código implementado em Spark é normalmente mais rápido que a implementação equivalente em MapReduce. Por quê?
R: Não tive entendimento suficiente para responder com clareza. 

- Qual é a função do SparkContext ?
R: Executar aplicações, chamar as "funções" e também o contexto geral, dando acesso aos recursos do
Spark.

- Explique com suas palavras o que é Resilient Distributed Datasets (RDD).
R: Estrutura principal do Spark, é como se fosse um dataframe do pandas, a diferença é que a RDD foi
criada para rodar em ambiente distribuído.

- GroupByKey é menos eficiente que reduceByKey em grandes dataset. Por quê?
R: Devido ao método de agrupamento das Keys. => reduceByKey faz o agrupamento das Keys primeiro, já no GroupByKey, o agrupamento,
é feito somente depois. Para grandes volumes, o ganho de desempenho com reduceByKey é maior.

- Explique o que o código Scala abaixo faz.
R: É um conta palavras. 
-Primeira linha: leitura dos dados/input
-Segunda linha: Separação por espaços e submetidos a uma sequencia de caracteres pelo flatMap
-Terceira linha: Utilizando o método map é atribuído um valor para cada chave
-Quarta linha: salvando o processo em um sistema distribuído.
