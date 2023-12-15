## Análise de ações com envelopes de médias móveis

Neste Jupyter Notebook fiz uma análise de ações utilizando Python, Pandas, NumPy, Matplotlib, SciPy e Yahoo Finance. A análise inclui a obtenção de preços históricos de ações via Yahoo Finance, a plotagem desses preços ao longo do tempo e a aplicação de envelopes de médias móveis para identificar possíveis sinais de compra ou venda.

### Instalação
Primeira passo no notebook é a instalação dos pacotes Python necessários, executando o seguinte comando:
<img width="988" alt="image1" src="https://github.com/mjr/investiment-analysis/assets/9324986/4a28cee4-5ef1-4c9b-9605-55c0c2d9be3b">

### Obtendo preços das ações
Na sequência busco os preços históricos das ações selecionadas (AAPL, MSFT, GOOG) no Yahoo Finance. O período de análise definido foi de "2023-06-14" a "2023-12-14".
Nesta etapa, os pacotes necessários são importados, e a função get_data_yahoo do pandas_datareader é utilizada para obter os preços de fechamento ajustados ("Adj Close") das ações da Apple (AAPL), Microsoft (MSFT) e Alphabet (GOOG) no período de 14 de junho de 2023 a 14 de dezembro de 2023.
<img width="980" alt="image2" src="https://github.com/mjr/investiment-analysis/assets/9324986/8f6899c4-6b97-4704-b7e8-2158efe2312e">

### Plotando preços de ações ao longo do tempo
Depois ploto os preços de fechamento ajustados ao longo do tempo para os ativos selecionados. Utilizo a biblioteca Matplotlib para criar um gráfico que mostra a evolução dos preços das ações durante o período analisado.
<img width="980" alt="image3" src="https://github.com/mjr/investiment-analysis/assets/9324986/edd0f7ea-cc55-44c3-9b2d-5e071903a7cc">

### Aplicando envelopes de médias móveis
Por fim aplico envelopes de médias móveis aos preços das ações para identificar tendências potenciais. Calculo as médias móveis simples (MMA) para cada ativo, utilizando uma janela de 20 períodos. Em seguida, crio um banda superior e uma inferior em torno da MMA, formando um "envelope" que pode indicar áreas de sobrecompra ou sobrevenda. No final ploto os preços das ações, as MMAs e os envelopes de MMAs para os ativos selecionados.
<img width="985" alt="image4" src="https://github.com/mjr/investiment-analysis/assets/9324986/73a3b4a5-f3a9-4ac5-93e8-247d0bbd506a">
