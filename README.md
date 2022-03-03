# Projeto-ETL-Consultas-SQL

Projeto de ETL e análise de dados desenvolvido em parceria com @LucasBrandaoGomes, @na-geciauskas e Iris Gassner. Tema do projeto: mudanças climáticas.

## Ferramentas utilizadas:
* Linguagem de programação Python
* Linguagem de programação SQL
* Bibliotecas Pandas, Pandera, PySpark e Matplotlib
* Google Cloud Storage e Big Query

## Datasets utilizados:
* Temperaturas médias por país de 1750 a 2013 (utilizados dados somente a partir de 1900)
* CO2 na atmosfera por país de 1750 a 2017
* Cobertura Florestal por país de 1985 a 2020

## Metodologia
* Processos ETL
  - Cada dataset foi tratado e normalizado em um notebook prórpio do google colaboratory
  - Com a biblioteca Pandas foram realizados os tratamentos básicos, como verificação de inconsistências, renomeação de colunas, apagar colunas ou linhas não úteis para análises
  - A validação dos dados foi realizada com a biblioteca Pandera
  - Os procedimentos de modelagem dos dados, bem como a criação de colunas interessantes para a análise foram realizados com o PySpark
  - Algumas tabelas foram tratadas para se chegar a uma tabela única, através da função join do PySpark
* Consultas e plotagens
  - Foram realizadas consultas prévias utilizando a sintaxe PySpark e SparkSQL
  - Foram realizadas plotagens com a biblioteca
* Google Cloud
  - Os arquivos foram armazenados no Google Cloud Storage, tanto as versões sem tratamento quanto as tratadas
  - O BigQuery foi utilizado como Data Warehouse, armazenando os arquivos tratados
  - No Big Query realizamos consultas SQL
  - A partir das consultas criamos dashboards com o Google Data Studio

## Dashboards
https://user-images.githubusercontent.com/98925230/156645308-62974847-ab56-4adb-86ad-02d49249b99c.mov

