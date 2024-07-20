# Projeto de Clusterização e Análise Exploratória de Clientes de um Mercado

### Autor: Pedro Lourenço Mendes Júnior

[Linkedin](https://www.linkedin.com/in/mendesjuniorpedro/)

## Introdução
Em um mundo cada vez mais **orientado por dados**, muitas empresas buscam extrair informações valiosas a partir dos dados que as cercam. Dado um número grande de informações, surgem possibilidades para que possamos compreender melhor o todo, encontrar alguns padrões, tendências, casos estranhos, etc. Nesse sentido, a **análise exploratória de dados** é uma etapa fundamental nesse processo, pois nos permite examinar e visualizar os padrões presentes nos dados, compreendendo assim as suas características e potencialidades. Além disso, os **modelos de machine learning** se popularizaram nos últimos anos com o avanço tecnológico e potencializaram a tomada de decisão por meio dos dados, o data-driven.

Os dados utilizados neste projeto são provenientes do [Kaggle.com](https://www.kaggle.com/) e podem ser acessados **[aqui](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)**. Trata-se de um conjunto de dados hipotéticos de clientes que realizaram compras em um determinado intervalo de tempo. Cada registro representa um cliente e as suas características, como idade, formação, salário, histórico de compras por departamento, visitas ao website da empresa, etc.

## Objetivos do Projeto
O principal objetivo deste projeto é aplicar técnicas de análise exploratória, limpeza e aprendizado de máquina para **segmentar os clientes em grupos distintos**. Isso permitirá compreender melhor o comportamento dos clientes e tomar decisões estratégicas para cada segmento.

## Dicionário de Dados
Aqui estão as principais variáveis utilizadas na análise:

| Variável           | Descrição                                                                                      |
|--------------------|------------------------------------------------------------------------------------------------|
| `ID`               | Identificador único do cliente                                                                 |
| `Year_Birth`       | Ano de nascimento do cliente                                                                   |
| `Education`        | Nível de educação do cliente                                                                   |
| `Marital_Status`   | Estado civil do cliente                                                                        |
| `Income`           | Renda anual do cliente                                                                         |
| `Kidhome`          | Número de crianças na casa                                                                     |
| `Teenhome`         | Número de adolescentes na casa                                                                 |
| `Dt_Customer`      | Data de inscrição do cliente                                                                   |
| `Recency`          | Dias desde a última compra                                                                     |
| `MntWines`         | Valor gasto em vinhos                                                                          |
| `MntFruits`        | Valor gasto em frutas                                                                          |
| `MntMeatProducts`  | Valor gasto em produtos de carne                                                               |
| `MntFishProducts`  | Valor gasto em produtos de peixe                                                               |
| `MntSweetProducts` | Valor gasto em produtos doces                                                                  |
| `MntGoldProds`     | Valor gasto em produtos de ouro                                                                |
| `NumDealsPurchases`| Número de compras com desconto                                                                 |
| `NumWebPurchases`  | Número de compras pela web                                                                     |
| `NumCatalogPurchases` | Número de compras por catálogo                                                              |
| `NumStorePurchases`| Número de compras na loja                                                                      |
| `NumWebVisitsMonth`| Número de visitas ao site por mês                                                              |
| `AcceptedCmp1`     | 1 se aceitou a oferta na campanha 1, 0 caso contrário                                          |
| `AcceptedCmp2`     | 1 se aceitou a oferta na campanha 2, 0 caso contrário                                          |
| `AcceptedCmp3`     | 1 se aceitou a oferta na campanha 3, 0 caso contrário                                          |
| `AcceptedCmp4`     | 1 se aceitou a oferta na campanha 4, 0 caso contrário                                          |
| `AcceptedCmp5`     | 1 se aceitou a oferta na campanha 5, 0 caso contrário                                          |
| `Response`         | 1 se aceitou a última campanha, 0 caso contrário                                               |
| `Complain`         | 1 se reclamou no último mês, 0 caso contrário                                                  |
| `Country`          | País do cliente                                                                                |

## Principais Análises e Resultados

### 1. Valor Total Gasto por Cluster
![Valor Total Gasto por Cluster](https://github.com/pedromendesjr/cluster-market/blob/main/imagens/total_gasto.png?raw=true)

O gráfico mostra a distribuição do valor total gasto por cluster. O Cluster 1 tem o maior gasto médio, seguido pelo Cluster 0 e, finalmente, pelo Cluster 2, que tem o menor gasto médio.

### 2. Número de Compras Realizadas por Cluster
![Número de Compras Realizadas por Cluster](https://github.com/pedromendesjr/cluster-market/blob/main/imagens/total_compras.png?raw=true)

O gráfico mostra a distribuição do número de compras realizadas por cluster. O Cluster 1 se destaca com o maior número de compras, enquanto o Cluster 2 tem o menor número de compras realizadas.

### 3. Renda Anual por Cluster
![Renda Anual por Cluster](https://github.com/pedromendesjr/cluster-market/blob/main/imagens/salario_cluster.png?raw=true)

O gráfico mostra a distribuição da renda anual por cluster. O Cluster 1 possui a maior renda média, o que pode explicar os altos gastos e número de compras, enquanto o Cluster 2 tem a menor renda média.

## Conclusão
Neste projeto, utilizamos técnicas de clusterização para segmentar os clientes de um mercado em três grupos distintos, com base em suas características de compra e renda. As principais observações são:

1. **Cluster 0**: Clientes com gastos e número de compras medianos. Este grupo possui uma renda média moderada.
2. **Cluster 1**: Clientes com os maiores gastos e número de compras. Este grupo tem a maior renda média, indicando um perfil de clientes de alto valor.
3. **Cluster 2**: Clientes com os menores gastos e número de compras. Este grupo tem a menor renda média, sugerindo um perfil de clientes de baixo valor.

A segmentação dos clientes em clusters distintos permite uma melhor compreensão de seu comportamento e a tomada de decisões estratégicas específicas para cada grupo. Por exemplo, campanhas de marketing mais agressivas podem ser direcionadas ao Cluster 1, enquanto estratégias de fidelização podem ser mais adequadas para o Cluster 0. O Cluster 2 pode beneficiar-se de ofertas e promoções para aumentar seu engajamento e valor de vida útil.

Esses resultados demonstram a importância de utilizar técnicas de aprendizado de máquina, como a clusterização, para entender melhor os clientes e otimizar estratégias de negócios.
