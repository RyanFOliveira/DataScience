# DataScience

📈 Análise de Ações da B3 com Aprendizado Supervisionado (2018–2021)
Este projeto utiliza técnicas de Data Science e Aprendizado Supervisionado para analisar e prever os preços de fechamento de ações da Bolsa de Valores Brasileira (B3) com base em dados históricos do período de 2018 a 2021.

📌 Objetivo
Prever o preço de fechamento de ações com base em atributos como preço de abertura, volume, ticker, e data, comparando diferentes algoritmos de regressão.

📊 Dataset
Fonte: Dados históricos da B3, entre 2018 e 2021.

Formato: .csv com as seguintes colunas:

ref.date, ticker, Empresa, Setor, price.open, price.close, volume, etc.

Pré-processamento:

Conversão de strings numéricas para float

Transformação de datas

Cálculo de variações e identificação de outliers

🧠 Modelos de Regressão Avaliados
Modelo	MSE	RMSE	MAE	R²
Regressão Linear	385.13	19.62	7.13	0.7415
Decision Tree	24.77	4.98	0.68	0.9834
Gradient Boosting	113.45	10.65	5.16	0.9239
Random Forest	20.00	4.47	0.63	0.9866

✅ Conclusão: O modelo Random Forest com hiperparâmetros otimizados teve o melhor desempenho, com excelente capacidade de generalização.

🔧 Tecnologias Utilizadas
Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)

Google Colab
