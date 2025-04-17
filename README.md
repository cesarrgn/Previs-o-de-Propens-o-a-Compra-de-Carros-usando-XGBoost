# Projeto de Propensão a Compra de Carros com XGBoost

Este projeto implementa um modelo de Machine Learning para prever a probabilidade de um cliente comprar um carro, utilizando o algoritmo XGBoost.

## 📌 Objetivo
Desenvolver um modelo preditivo que:
- Classifique clientes em "propensos a comprar" (1) ou "não propensos" (0)
- Identifique as variáveis mais importantes na decisão de compra
- Atingir alta acurácia (>80%) na previsão

## 📋 Metodologia
1. **Pré-processamento**:
   - Label Encoding para variáveis categóricas
   - Remoção de colunas irrelevantes (ID)
   - Análise de correlação entre features

2. **Modelagem**:
   - Algoritmo: XGBoost Classifier
   - Hyperparâmetros:
     - `max_depth=3`
     - `learning_rate=0.1`
     - `n_estimators=100`

3. **Avaliação**:
   - Acurácia: 83.33%
   - Matriz de Confusão
   - Feature Importance

## 📊 Resultados
| Métrica         | Valor  |
|-----------------|--------|
| Acurácia        | 83.33% |
| Precision (Classe 1) | 73%   |
| Recall (Classe 1)    | 70%   |

**Variáveis mais importantes**:
1. Salary (45)
2. Age (32)
3. Gender_encoded (23)

## 🛠️ Como Executar
1. Instale as dependências:
```bash
pip install pandas numpy xgboost scikit-learn matplotlib seaborn
