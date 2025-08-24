# 🤖 Modelagem de Dados - Capítulo 1

## Introdução à Modelagem
Técnicas para criar modelos preditivos e analíticos.

## Tipos de Modelos
- Regressão (linear, logística)
- Classificação
- Clusterização
- Redução de dimensionalidade

## Workflow Básico
1. Divisão treino/testeddddd
2. Seleção de features
3. Treinamento do modelo
4. Avaliação de performance
5. Otimização de hiperparâmetros

## Exemplo: Regressão Linear
```python
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)

model = LinearRegression()
model.fit(X_train, y_train)

predictions = model.predict(X_test)