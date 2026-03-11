# 📈 Análise de Ações da B3 com Machine Learning

Este projeto aplica técnicas de **Data Science e Machine Learning supervisionado** para analisar e prever o **preço de fechamento de ações da Bolsa de Valores Brasileira (B3)** utilizando dados históricos entre **2018 e 2021**.

---

## 🎯 Objetivo

Desenvolver modelos de **regressão supervisionada** capazes de prever o **preço de fechamento das ações**, utilizando variáveis como:

- preço de abertura
- volume de negociação
- ticker da ação
- data
- outros indicadores derivados

O projeto também compara o desempenho de diferentes algoritmos de **Machine Learning**.

---

## 📊 Dataset

**Fonte:** Dados históricos da B3  
**Período:** 2018 – 2021  

Formato `.csv` contendo colunas como:

- `ref.date`
- `ticker`
- `empresa`
- `setor`
- `price.open`
- `price.close`
- `volume`

---

## 🧹 Pré-processamento de Dados

Etapas aplicadas antes da modelagem:

- Conversão de **strings numéricas para float**
- Transformação e manipulação de **datas**
- Criação de **features derivadas**
- Identificação e tratamento de **outliers**
- Preparação dos dados para algoritmos de regressão

---

## 🤖 Modelos de Machine Learning Avaliados

| Modelo | MSE | RMSE | MAE | R² |
|------|------|------|------|------|
| Regressão Linear | 385.13 | 19.62 | 7.13 | 0.7415 |
| Decision Tree | 24.77 | 4.98 | 0.68 | 0.9834 |
| Gradient Boosting | 113.45 | 10.65 | 5.16 | 0.9239 |
| Random Forest | **20.00** | **4.47** | **0.63** | **0.9866** |

---

## 📈 Resultados

O modelo **Random Forest com hiperparâmetros otimizados** apresentou o melhor desempenho entre os modelos testados, alcançando:

- **R² = 0.9866**
- **RMSE = 4.47**

Isso indica **alta capacidade de generalização** na previsão dos preços de fechamento das ações.

---

## 🛠️ Tecnologias Utilizadas

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Google Colab**

---

## 🚀 Possíveis Melhorias

- Inclusão de **dados macroeconômicos**
- Testar modelos de **Deep Learning (LSTM para séries temporais)**
- Implementação de **pipeline automatizado de dados**
- Deploy de modelo para **previsão em tempo real**
