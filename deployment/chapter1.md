# 🚀 Deployment de Modelos - Capítulo 1

## O que é Deployment?
Colocar modelos em produção para uso real.

## Opções de Deployment
- APIs REST (FastAPI, Flask)
- Serviços cloud (AWS SageMaker, Azure ML)
- Containers Docker
- Streaming (Kafka, Spark Streaming)

## Exemplo: API com FastAPI
```python
from fastapi import FastAPI
import pickle

app = FastAPI()

# Carrega modelo treinado
with open('modelo.pkl', 'rb') as f:
    model = pickle.load(f)

@app.post("/predict")
def predict(data: dict):
    prediction = model.predict([data['features']])
    return {"prediction": prediction.tolist()}