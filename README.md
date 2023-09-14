# F1RST-Diario-de-Bordo
 Repositório referente ao segundo módulo do desafio técnico da F1RST - São Carlos: Diário de Bordo

A amostra de dados (info_transportes.csv), possui dados de um
aplicativo de transporte privado, cujas colunas são:

- DATA_INICIO (formato: "mm-dd-yyyy HH")

- DATA_FIM (formato: "mm-dd-yyyy HH")

- CATEGORIA

- LOCAL_INICIO

- LOCAL_FIM

- PROPOSITO

- DISTANCIA

Uma equipe está elaborando um modelo para compreender como os clientes
estão utilizando o aplicativo. Para isso, você precisa fornecer uma nova tabela
“info_corridas_do_dia", com dados agrupados pela data de início do transporte
utilizando a formatação “yyyy-MM-dd”, contendo as seguintes colunas:

| Nome da Coluna      | Descrição                                                             |
|---------------------|-----------------------------------------------------------------------|
| DT_REFE             | Data de referência.                                                   |
| QT_CORR             | Quantidade de corridas.                                               |
| QT_CORR_NEG         | Quantidade de corridas com a categoria "Negócio".                      |
| QT_CORR_PESS        | Quantidade de corridas com a categoria "Pessoal".                      |
| VL_MAX_DIST         | Maior distância percorrida por uma corrida.                            |
| VL_MIN_DIST         | Menor distância percorrida por uma corrida.                            |
| VL_AVG_DIST         | Média das distâncias percorridas.                                       |
| QT_CORR_REUNI       | Quantidade de corridas com o propósito de "Reunião".                   |
| QT_CORR_NAO_REUNI   | Quantidade de corridas com o propósito declarado e diferente de "Reunião".|


Abaixo temos um exemplo de uma possível linha da tabela:

| DT_REFE      | QT_CORR | QT_CORR_NEG | QT_CORR_PESS | VL_MAX_DIST | VL_MIN_DIST | VL_AVG_DIST | QT_CORR_REUNI | QT_CORR_NAO_REUNI |
|--------------|---------|-------------|--------------|------------|------------|------------|--------------|------------------|
| 2022-01-01   | 20      | 12          | 8            | 2.2        | 0.7        | 1.1        | 6            | 10               |

O código que você irá elaborar para criar a tabela (ou dataframe spark/pandas)
deverá ser escrito em uma das seguintes linguagens: SQL ou Python
(pyspark e/ou pandas). Caso decida por SQL, considere o nome da tabela
como " info_transportes".

***


## Requisitos

Para executar este projeto, você precisará ter as seguintes bibliotecas instaladas:

- [pyspark](https://pypi.org/project/pyspark/)
- [pandas](https://pypi.org/project/pandas/)

## Instalação

Você pode instalar as bibliotecas utilizando o pip. Abra o terminal ou prompt de comando e execute os seguintes comandos:

```bash
pip install pyspark
pip install pandas
