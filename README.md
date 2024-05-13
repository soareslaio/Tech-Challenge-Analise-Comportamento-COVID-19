# Tech-Challenge-3-Analise-Comportamento-COVID-19
Analisar o comportamento da população durante a pandemia do COVID - 19

**Objetivo:**  Elabore 20 perguntas que respondam: Quais seriam o comportamento da população na época da pandemia da COVID - 19, Caracteristicas Clinicas dos sintomas, caracteristicas da população, caracteristiacas economicas da sociedade? Além de elaborar principais ações que o hospital deverá tomar em caso de um novo surto de COVID - 19.

**Regras:**

1) Utilização de no máximo 20 questionamentos realizados na pesquisa;
2) Utilizar 3 meses para construção da solução;
3) Caracterização dos sintomas clínicos das população;
4) Comportamento da população na época do COVID - 19;
5) Características econômicas da Sociedade;

**Pesquisa Nacional por Amostra de Domicílios (PNAD)**
A PNAD, conduzida pelo IBGE, investiga várias características da população brasileira, incluindo educação, trabalho, rendimento e habitação.

**Características da População Analisadas**
  - Mapeamento da situação domiciliar e tipos de área, incluindo áreas urbanas e regiões específicas.
  - Demografia: sexo, cor ou raça, e faixa etária dos entrevistados.
  - Educação: frequência escolar e escolaridade.
  - Participação em aulas presenciais durante a pandemia.
    
**Principais Resultados**
  - Maioria dos entrevistados residia em áreas urbanas, principalmente nas capitais estaduais.
  - Predominância de mulheres, faixa etária entre 10 e 60 anos, e cor predominante branca ou parda.
  - Grande parte possuía ensino fundamental incompleto ou médio completo, e a maioria frequentou aulas presenciais ou semipresenciais durante a pandemia.
    
**Sintomas e Doenças Preexistentes**
  - Principais sintomas para casos positivos de COVID-19 incluíam dor de cabeça, tosse e febre. Cerca de um terço dos entrevistados relatou ter doenças prévias, como hipertensão e diabetes.

**Medidas e Acesso à Saúde**
  - A maioria adotou medidas restritivas para evitar a propagação do vírus.
  - Acesso aos serviços de saúde, com destaque para o Sistema Único de Saúde (SUS).
  - Preferência por testes rápidos e suas implicações na detecção precoce.
    
**Modelo Preditivo e Conclusões**
  - Utilização de dados da PNAD para desenvolver um modelo preditivo de infecção por COVID-19.
  - Análise estatística e modelagem para prever resultados de testes de COVID-19 com base em características demográficas e condições pré-existentes.
  - Resultados do modelo indicaram uma capacidade sólida de previsão, com espaço para otimização contínua.
    
Análise aprofundada: https://medium.com/@laiosoares6/objetivo-analisar-dados-da-pnad-durante-a-pandemia-covid-19-e-analisar-comportamentos-e-poss%C3%ADveis-956c107c3bd4

**Pipeline para analise de dados**

![alt text](https://github.com/soareslaio/Tech-Challenge-Analise-Comportamento-COVID-19/blob/main/Fluxograma_analise_dados/analise_dados_pnad_covid19.png?raw=true)

1) Extraido base de dados no formato .CSV do IBGE PNAD COVID19
2) Feito a ingestão do .CSV dentro do Google Colar.
4) Transformado em arquivo .PARQUET para poupar armazenamento e processamento de maquina, uma vez que o formato .parquet é colunar.
5) Feito upload dos arquivos .parquet para o Github
6) Google colab para consumir os arquivos direto do Github
7) Realizado o ETL para tratar os dados do IBGE
8) Realizado as analises exploratorios para extração de ideias para o tema proposto
9) Elaborado o documento final com as analises realizadas.
