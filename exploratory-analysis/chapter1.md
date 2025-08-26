# 🔍 Análise Exploratória de Dados - Capítulo 1

## Introdução
A análise exploratória é a primeira etapa para entender os dados, identificar padrões e detectar anomaliasddddd.

## Técnicas Principais

### Estatística Descritiva
- Medidas de tendência central: média, mediana, moda
- Medidas de dispersão: variância, desvio padrão, amplitude
- Quartis e percentis

### Visualização de Dados
- Histogramas para distribuições
- Boxplots para identificar outliers
- Scatter plots para relações entre variáveis

## Exemplo Prático
```python
import pandas as pd
import matplotlib.pyplot as plt

# Estatísticas descritivas
print(df.describe())

# Histograma
df['coluna_numerica'].hist()
plt.title('Distribuição dos Dados')
plt.show()