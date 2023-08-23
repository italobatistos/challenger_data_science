# Desafio Cientista de Dados - Séries temporais

**Crescimento do índice do GDP para os anos 2024-2028**

## Contextualização:

_""Na maioria dos anos desde 1980, o crescimento do PIB global tem sido relativamente consistente, geralmente flutuando entre dois e cinco por cento de crescimento de ano para ano. As exceções mais notáveis ​​​​a isso foram durante a Grande Recessão em 2009 e novamente em 2020 durante o Covid- 19, onde a economia global realmente encolheu em ambos os anos. Enquanto a economia mundial continua a lidar com o impacto econômico da pandemia, bem como as consequências da invasão russa da Ucrânia em 2022, o futuro permanece incerto, porém atual estimativas sugerem que o crescimento anual retornará a valores estáveis ​​de cerca de 3% em 2028."_

_Aaron O'Neill, 10 de maio de 2023."_

## Desafio :

O desafio visa avaliar o desenvolvimento de um EDA (análise exploratória de dados) e os conhecimentos/insights relacionados a um tipo clássico de problema de ciência de dados: séries temporais. Para isso, gostaria de ver o crescimento do índice do PIB de cada país nos anos 2024-2028, comparando-os posteriormente com o previsto pelo Statistica. Além disso, é necessário substituir os campos "no data" por valores numéricos, utilizando as inferências de sua preferência.

-------------------

## Objetivo :

Prever o crescimento do índice do PIB de cada país nos anos 2024-2028.

## Fluxo de Análise:

 * 1. Importe as bibliotecas necessárias
 * 2. Leia e entenda os dados
 * 3. Análise Exploratória de Dados
 * 4. Preparação de Dados
 * 5. Decomposição da série temporal
 * 6. Criando e avaliando a previsão de séries temporais

## Desempenho do Modelo ARIMA

Foi realizado um estudo de previsão de séries temporais utilizando o modelo ARIMA (AutoRegressive Integrated Moving Average) com otimização automática de parâmetros usando a função auto_arima.

**Configuração do Modelo:**

Modelo: ARIMA
Método de Otimização de Parâmetros: **auto_arima**
Métrica de Avaliação: MAPE (Mean Absolute Percentage Error)

**Resultado:**

A média de MAPE obtida para as previsões utilizando o modelo ARIMA foi de 30%.

**Observações:**

O modelo ARIMA foi escolhido devido à sua capacidade de lidar com séries temporais univariadas e à otimização automática de parâmetros.
O MAPE é uma métrica comumente usada para avaliar o desempenho de modelos de previsão, representando a porcentagem média de erro absoluto em relação aos valores reais.
O valor de MAPE de 30% indica que, em média, as previsões do modelo ARIMA têm um erro absoluto médio de 30% em relação aos valores reais.
Este resultado fornece uma avaliação do desempenho do modelo ARIMA em suas previsões e pode ser usado para tomar decisões informadas sobre sua utilidade em cenários específicos.

## Autor

* [Italo Batista](https://www.linkedin.com/in/italobatista/)

## Reconhecimentos

* **Alisson Louly**
* **Leo Michel**
* **Lucas Dias**
