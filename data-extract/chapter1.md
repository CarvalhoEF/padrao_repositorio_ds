# 📥 Extração de Dados - Capítulo 1

## Introdução à Extração de Dados
Técnicas e ferramentas para coleta de dados de diversas fontes.

## Fontes de Dados Comuns
- Bancos de Dados SQL e NoSQL
- APIs RESTful e GraphQL
- Web Scraping
- Arquivos (CSV, JSON, Excel)
- Streams de dados em tempo real

## Ferramentas Principais
```python
# Exemplo: Extração com Pandas
import pandas as pd

# CSV
df = pd.read_csv('dados.csv')

# Excel
df = pd.read_excel('dados.xlsx')

# Banco SQL
import sqlalchemy
engine = sqlalchemy.create_engine('sqlite:///banco.db')
df = pd.read_sql('SELECT * FROM tabela', engine)