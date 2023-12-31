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

 * Importe as bibliotecas necessárias
 * Leia e entenda os dados
 * Análise Exploratória de Dados
 * Preparação de Dados
 * Decomposição da série temporal
 * Criando e avaliando a previsão de séries temporais

## Desempenho do Modelo ARIMA

Foi realizado um estudo de previsão de séries temporais utilizando o modelo ARIMA (AutoRegressive Integrated Moving Average) com otimização automática de parâmetros usando a função auto_arima.

**Configuração do Modelo:**

Modelo: **ARIMA**

Método de Otimização de Parâmetros: **auto_arima**

Métrica de Avaliação: **MAPE (Mean Absolute Percentage Error)**

**Resultado:**

A média de MAPE obtida para as previsões utilizando o modelo ARIMA foi de 31%.

**Observações:**

  * O modelo ARIMA foi escolhido devido à sua capacidade de lidar com séries temporais univariadas e à otimização automática de parâmetros.
  * O MAPE é uma métrica comumente usada para avaliar o desempenho de modelos de previsão, representando a porcentagem média de erro absoluto em relação aos valores reais.
  * O valor de MAPE de 31% indica que, em média, as previsões do modelo ARIMA têm um erro absoluto médio de 31% em relação aos valores reais.
    
Este resultado fornece uma avaliação do desempenho do modelo ARIMA em suas previsões e pode ser usado para tomar decisões informadas sobre sua utilidade em cenários específicos.

Além do resultado do MAPE, é importante analisar o desempenho do modelo ARIMA por meio dos gráficos gerados. Abaixo estão algumas observações sobre o resultado dos gráficos obtidos:

**Comparação Visual:** Os gráficos de previsão versus valores reais permitem uma comparação visual direta do desempenho do modelo. Se as previsões estiverem bem alinhadas com os valores reais, isso é um indicativo positivo do modelo.

**Tendências e Sazonalidade:** Ao observar os gráficos, é importante verificar se o modelo ARIMA capturou com precisão as tendências e sazonalidades nos dados. Isso é crucial para fazer previsões precisas.

**Erros e Discrepâncias:** Em alguns casos, é possível observar discrepâncias significativas entre as previsões e os valores reais. Essas discrepâncias podem ser áreas de melhoria no modelo. É importante examinar essas áreas com cuidado para entender a causa das diferenças.

**Variações ao Longo do Tempo:** Os gráficos podem mostrar se o desempenho do modelo é consistente ao longo do tempo ou se há variações significativas em diferentes períodos. Essa análise ajuda a identificar se o modelo é mais eficaz em determinadas condições ou períodos.

**Impacto do MAPE:** O MAPE, como mencionado, fornece uma métrica quantitativa do desempenho médio do modelo. É útil para resumir o erro médio em uma única medida, mas também é importante considerar como esse erro se distribui ao longo do tempo.

Lembrando que o MAPE de 37% indica um erro médio absoluto de 37% em relação aos valores reais. Isso pode ser considerado alto ou baixo dependendo do contexto específico da aplicação e das expectativas de precisão.

Portanto, além do MAPE, a análise visual dos gráficos é fundamental para avaliar a capacidade do modelo ARIMA de fornecer previsões precisas e identificar possíveis áreas de melhoria ou ajuste do modelo.

Em conclusão, a previsão do índice de Produto Interno Bruto (PIB) é uma tarefa crucial para muitos setores, incluindo negócios, governo e finanças. Embora tenhamos explorado a utilização do modelo ARIMA como uma ferramenta valiosa para esse propósito, é importante reconhecer que há espaço para melhorias significativas na precisão das previsões.

Um estudo mais aprofundado no futuro pode ser extremamente benéfico para aprimorar o desempenho do modelo ARIMA. Isso envolveria a consideração de vários aspectos, incluindo:

 * **Dados de alta qualidade:** Certificar-se de que os dados utilizados para a modelagem são precisos e atualizados é fundamental. Qualquer erro ou falta de dados pode afetar drasticamente a acuracidade das previsões.

 * **Tratamento de outliers robusto:** A detecção e tratamento adequado de outliers são essenciais. Explorar métodos mais avançados, como o uso de modelos robustos, pode ajudar a lidar com valores discrepantes de maneira mais eficaz.

 * **Imputação de dados:** A imputação de dados ausentes ou inconsistentes é um desafio comum em análises de séries temporais. Considere abordagens mais sofisticadas para imputação, como a utilização de técnicas de aprendizado de máquina, para melhorar a integridade dos dados.

 * **Seleção de características:** Avaliar se todas as variáveis utilizadas na modelagem são relevantes e contribuem efetivamente para a precisão das previsões. A seleção de características pode simplificar o modelo e reduzir o risco de overfitting.

 * **Experimentação com outros modelos:** Além do ARIMA, considere explorar outros modelos de séries temporais, como modelos de médias móveis exponenciais (EMA), modelos de suavização exponencial, ou mesmo técnicas de aprendizado de máquina, como redes neurais, para ver se eles oferecem desempenho superior em suas previsões.

 * **Avaliação contínua:** Monitorar regularmente o desempenho do modelo e ajustá-lo conforme necessário à medida que mais dados se tornam disponíveis ou à medida que as condições econômicas mudam.

Em suma, enquanto o modelo ARIMA é um ponto de partida valioso para prever o índice de PIB, um esforço contínuo para aprimorar sua precisão é essencial. Isso pode ser alcançado por meio de um estudo mais profundo dos dados, um tratamento de outliers mais robusto, aprimoramento na imputação de dados e a consideração de outros modelos de previsão. Com essas melhorias, você estará mais bem preparado para tomar decisões informadas e estratégicas em relação às tendências econômicas futuras.

## Autor

* [Italo Batista](https://www.linkedin.com/in/italobatista/)

## Reconhecimentos

* **Alisson Louly**
* **Leo Michel**
* **Lucas Dias**
* **Luzia Souza**
* **Lucas Sabino**
  
## Links:


*   https://analisemacro.com.br/data-science/python/estacionariedade_series_temporais/#:~:text=Caso%203%3A%20KPSS%20indica%20estacionariedade,a%20nova%20s%C3%A9rie%20%C3%A9%20estacion%C3%A1ria.
*   http://leg.ufpr.br/~lucambio/STemporais/STemporaisIII.html
*   https://medium.com/analytics-vidhya/time-series-forecasting-a-complete-guide-d963142da33f

