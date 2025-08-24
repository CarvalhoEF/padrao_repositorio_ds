# 🧹 Limpeza de Dados - Capítulo 1

## Importância da Limpeza
Dados limpos são essenciais para análise e modelagem precisas.
ghdgfjdhsfgsjhdgfhdjfghjd
## Problemas Comuns
- Valores missing (NaN, null, vazios)
- Outliers e valores extremos
- Inconsistências em dados categóricos
- Duplicatas
- Erros de formatação

## Técnicas de Tratamento
```python
import pandas as pd
import numpy as np

# Tratamento de missing values
df['coluna'].fillna(df['coluna'].mean(), inplace=True)

# Remoção de duplicatas
df.drop_duplicates(inplace=True)

# Identificação de outliers
Q1 = df['coluna'].quantile(0.25)
Q3 = df['coluna'].quantile(0.75)
IQR = Q3 - Q1