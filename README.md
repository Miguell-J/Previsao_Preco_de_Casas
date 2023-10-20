# Previsão do preço de casas

<img src="https://www.bi4all.pt/app/uploads/2020/06/vantagens-ai-2.png"/>

Este README fornece uma visão geral do código Python para prever os preços de casas usando várias técnicas de aprendizado de máquina e deep learning com o TensorFlow. O código carrega um conjunto de dados, o pré-processa, treina diferentes modelos e avalia seu desempenho usando várias métricas. Também inclui uma visualização das previsões dos modelos.

## Tabela de Conteúdo
- Introdução
- Visão Geral do Código
- Uso
- Dependências
- Licença

## Introdução
O código Python fornecido tem como objetivo prever os preços de casas usando uma combinação de técnicas de aprendizado de máquina e deep learning. Ele utiliza bibliotecas como TensorFlow, scikit-learn e pandas para carregar, pré-processar e modelar os dados. O código treina quatro modelos diferentes e avalia seu desempenho usando métricas como Erro Médio Absoluto (MAE) e Erro Quadrático Médio (MSE). Além disso, o código inclui uma representação visual das previsões dos modelos para comparação.

## Visão Geral do Código
O código pode ser resumido da seguinte maneira:

Carregamento e Pré-processamento dos Dados:

<img src="dataset house prediction.png"/>

- Carrega os dados de preços de casas de uma fonte online usando o pandas.
- Inspeciona o conjunto de dados para identificar valores ausentes e seleciona colunas com um número significativo de valores ausentes para remoção.
- Trata os valores ausentes preenchendo-os com um valor padrão (-1).
- Divide os dados em recursos de entrada (x) e variável alvo (y).
- Divide os dados em conjuntos de treinamento e teste usando train_test_split.

### Modelo de Regressão Linear:

- Treina um modelo de Regressão Linear usando o scikit-learn.
- Calcula previsões e avalia o desempenho do modelo usando MAE e MSE.

### Modelo de Árvore de Decisão:

- Treina um modelo de Regressor de Árvore de Decisão usando o scikit-learn.
- Calcula previsões e avalia o desempenho do modelo usando MAE e MSE.

### Modelo de Vizinhos Mais Próximos (KNN):

- Treina um modelo de Regressor de Vizinhos Mais Próximos (KNN) usando o scikit-learn.
- Calcula previsões e avalia o desempenho do modelo usando MAE e MSE.

### Modelo de Deep Learning (TensorFlow):

- Constrói um modelo de rede neural profunda usando a API Keras do TensorFlow.
- Compila o modelo com um otimizador Adam e função de perda MAE.
- Treina o modelo por 200 épocas.
- Calcula previsões para o conjunto de teste e avalia o desempenho do modelo usando MAE e MSE.

## Visualização:


<img src="Gráfico do house prediction.png"/>


- Visualiza as previsões dos quatro modelos usando gráficos de dispersão.
- Compara as previsões com os preços reais.

## Uso
Para usar este código, siga estas etapas:

- Instale as dependências necessárias listadas na próxima seção.

- Copie e cole o código em um ambiente Python, como Jupyter Notebook ou um script Python.

- Execute o código para carregar o conjunto de dados, pré-processá-lo, treinar os modelos e gerar métricas de desempenho e visualizações.

- Interprete os resultados para determinar qual modelo funciona melhor para a tarefa de previsão de preços de casas.

## Dependências
O código depende das seguintes bibliotecas e ferramentas Python:

- TensorFlow
- scikit-learn
- pandas
- matplotlib

## Licença
Este código é disponibilizado sob uma licença de código aberto. Você tem a liberdade de usá-lo, modificá-lo e distribuí-lo de acordo com os termos das respectivas licenças das bibliotecas e ferramentas usadas.

Verifique as licenças do TensorFlow, scikit-learn, pandas e matplotlib para obter mais detalhes.
