# Tech-Challenge-3-Analise-Comportamento-COVID-19
Analisar o comportamento da população durante a pandemia do COVID - 19

**Objetivo:** Analisar dados da PNAD durante a pandemia Covid-19 e analisar comportamentos e possíveis soluções caso tenha um novo surto.

**Características da população**
  - Mapeamento da situação domiciliar e tipos de área, incluindo áreas urbanas e regiões específicas.
  - Demografia: sexo, cor ou raça, e faixa etária dos entrevistados.
  - Educação: frequência escolar e escolaridade.
  - Participação em aulas presenciais durante a pandemia.

**Características econômicas da população**
- A maioria (75%) dos entrevistados recebeu alguma forma de renda do governo, como aposentadoria, pensão ou auxílios.
- A média de renda desses beneficiários foi de R$ 1.145,89, 4,17% superior ao salário mínimo vigente na época.
- Cerca de 20% dos entrevistados receberam dois ou mais benefícios.
- Aproximadamente 70% das pessoas trabalharam de forma remota durante a pandemia.
- Predominância de faixas de rendimento entre R$ 801 a R$ 1.600 e de R$ 1.600 a R$ 3.000 entre os entrevistados.
  
**Principais Resultados**
  - Maioria dos entrevistados residia em áreas urbanas, principalmente nas capitais estaduais.
  - Predominância de mulheres, faixa etária entre 10 e 60 anos, e cor predominante branca ou parda.
  - Grande parte possuía ensino fundamental incompleto ou médio completo, e a maioria frequentou aulas presenciais ou semipresenciais durante a pandemia.
    
**Sintomas e Doenças Preexistentes**
  - Principais sintomas para casos positivos de COVID-19 incluíam dor de cabeça, tosse e febre. Cerca de um terço dos entrevistados relatou ter doenças prévias, como hipertensão e diabetes.

**Medidas e Acesso à Saúde**
  - A maioria adotou medidas restritivas para evitar a propagação do vírus.
  - Acesso aos serviços de saúde, com destaque para o Sistema Único de Saúde (SUS).
  - Preferência por testes rápidos.
    
**Modelo Preditivo e Conclusões**
  - Utilização de dados da PNAD para desenvolver um modelo preditivo de infecção por COVID-19.
  - Análise estatística e modelagem para prever resultados de testes de COVID-19.
  - Resultados do modelo indicaram uma capacidade sólida de previsão, com espaço para otimização contínua.
    
Análise aprofundada: https://medium.com/@laiosoares6/objetivo-analisar-dados-da-pnad-durante-a-pandemia-covid-19-e-analisar-comportamentos-e-poss%C3%ADveis-956c107c3bd4

**Pipeline para analise de dados**

![alt text](https://github.com/soareslaio/Tech-Challenge-Analise-Comportamento-COVID-19/blob/main/Fluxograma_analise_dados/analise_dados_pnad_covid19.png?raw=true)

Durante o desenvolvimento do projeto foi analisado dentro do Bigquery a estrutura dos dados e também qual seria o pipeline para a entrega final. Mas optamos por seguir com a solução acima, pois era a mais eficiente para o objetivo do projeto, uma vez que ao importar os dados no formato .parquet diretamente do GitHub mostrou ser mais veloz do que diretamente do BigQuery para o Google Colab.

1) Extraído base de dados no formato .CSV do site do IBGE PNAD COVID19
2) Feito a ingestão do .CSV dentro do Google Colab.
4) Transformado em arquivo .PARQUET para poupar armazenamento e processamento de máquina, uma vez que o formato .parquet é colunar.
5) Feito upload dos arquivos .parquet para o Github
6) Google colab para consumir os arquivos direto do Github
7) Realizado o ETL para tratar os dados do IBGE
8) Realizado as análises exploratórios para extração de ideias para o tema proposto
9) Elaborado os documentos finais com as análises realizadas.
