# Projeto de Previsão de Séries Temporais com Deep Learning

Este repositório contém experimentos e códigos para previsão de séries temporais utilizando modelos estatísticos e de deep learning, com foco em aplicações de medição virtual de fluxo (Virtual Flow Metering) em dados industriais.

## Ambiente de Execução

Os experimentos foram realizados no [Google Colab](https://colab.research.google.com/) utilizando acelerador de GPU, o que permite treinar modelos de deep learning de forma eficiente.

## Estrutura do Projeto

- **data/**: Conjunto de dados utilizados nos experimentos (`train_data_scaled.csv`, `test_data_scaled.csv`, `riser_pq_uni.csv`).
- **notebooks/**: Notebooks Jupyter organizados em:
  - `notebooks-article/`: Notebooks para artigos científicos.
  - `notebooks-presentation/`: Notebooks para apresentações, separados por tipo de abordagem (univariada, exógena, multivariada).
- **models/**: Diretório para salvar modelos treinados.
- **results/**: Resultados dos experimentos, logs de otimização e métricas.
- **articles/**: Artigos e documentos relacionados ao projeto.

## Modelos e Abordagens

O projeto explora diferentes abordagens para previsão de séries temporais:
- Modelos estatísticos clássicos (ARIMA, SeasonalNaive, etc).
- Modelos de deep learning: NHITS, NBEATSx, LSTM, GRU, MLP, TCN, TFT, NLinear, StemGNN.
- Otimização de hiperparâmetros com Ray Tune e HyperOpt.

## Principais Frameworks Utilizados

- [NeuralForecast](https://github.com/Nixtla/neuralforecast)
- [StatsForecast](https://github.com/Nixtla/statsforecast)
- [scikit-learn](https://scikit-learn.org/)
- [feature-engine](https://feature-engine.readthedocs.io/)
- [Ray Tune](https://docs.ray.io/en/latest/tune/)
- [pandas](https://pandas.pydata.org/)
- [numpy](https://numpy.org/)
- [matplotlib](https://matplotlib.org/)

## Como Reproduzir

1. Acesse os notebooks em `notebooks/notebooks-article/` ou `notebooks/notebooks-presentation/` diretamente pelo [Google Colab](https://colab.research.google.com/), fazendo upload do notebook desejado ou conectando o repositório ao Colab.
2. Certifique-se de selecionar o acelerador de GPU em 'Ambiente de execução' > 'Alterar tipo de ambiente de execução'.
3. Os dados de entrada estão na pasta `data/` (faça upload para o ambiente do Colab, se necessário).
4. Execute as células dos notebooks para reproduzir os experimentos.
5. Os resultados e modelos treinados serão salvos nas pastas `results/` e `models/` (faça download dos arquivos gerados, se desejar mantê-los localmente).

## Artigos Relacionados

- [A Machine Learning Approach for Virtual Flow Metering and Forecasting](articles/A%20Machine%20Learning%20Approach%20for%20Virtual%20Flow%20Metering%20and%20Forecasting.pdf)

