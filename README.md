# Housing Prediction - Boston Dataset

## Descrição do Projeto
Este projeto utiliza o conjunto de dados de habitação de Boston (**Boston Housing Dataset**) do Scikit-Learn para construir um modelo de Machine Learning capaz de prever os preços das casas com base em diversas variáveis socioeconômicas e estruturais.

## Dataset
O conjunto de dados contém 506 amostras com 13 atributos numéricos que descrevem diferentes aspectos das residências e da localização, como:

- **CRIM**: Taxa de criminalidade per capita na cidade.
- **ZN**: Proporção de terrenos residenciais com mais de 25.000 pés quadrados.
- **INDUS**: Proporção de acres comerciais por cidade.
- **CHAS**: Variável dummy (1 se faz fronteira com o rio Charles, 0 caso contrário).
- **NOX**: Concentração de óxidos de nitrogênio (ppm).
- **RM**: Média do número de cômodos por residência.
- **AGE**: Proporção de unidades ocupadas pelos proprietários construídas antes de 1940.
- **DIS**: Distância ponderada para cinco centros de emprego de Boston.
- **RAD**: Índice de acessibilidade a rodovias radiais.
- **TAX**: Taxa de imposto sobre propriedade por $10.000.
- **PTRATIO**: Razão aluno-professor por cidade.
- **B**: Proporção de pessoas negras por cidade.
- **LSTAT**: Percentual da população de baixa renda.

O alvo (**target**) representa o valor médio das casas ocupadas pelos proprietários (em milhares de dólares).

## Tecnologias Utilizadas
- Python 3.x
- Scikit-Learn
- XGBoost
- Pandas
- NumPy

## Modelagem
Foram testados três modelos de aprendizado de máquina:
- **Regressão Linear** (LinearRegression - Scikit-Learn)
- **Support Vector Regression** (SVR - Scikit-Learn)
- **Decision Tree Regression** (XGBoost)

Assumimos que todas as variáveis são numéricas e aplicamos pré-processamento adequado.

### Test Design:
- **Divisão do Dataset**: 80% treino e 20% teste (via Scikit-Learn)
- **Métricas de avaliação**:
  - **Mean Squared Error (MSE)**
  - **Root Mean Squared Error (RMSE)**

### Otimização de Hiperparâmetros:
- Utilizando o método **GridSearchCV** do Scikit-Learn para encontrar os melhores parâmetros para os modelos.

## Resultados
Os resultados obtidos mostraram que o modelo conseguiu capturar a relação entre os atributos e o preço das casas, conforme demonstrado pelas métricas de avaliação.

## Licença
Este projeto está sob a licença MIT.

