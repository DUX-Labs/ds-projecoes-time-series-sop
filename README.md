# Modelo de Projeção de Demanda - S&OP por Canal

Notebook para desenvolvimento e aplicação de modelos de previsão de vendas segmentados por canal e subfamília de produto, utilizando séries temporais.

## Objetivo

Gerar projeções de vendas com modelos de Machine Learning gerados no python (LightGBM, XGBoost, RandomForest) e otimizados via Optuna, além de modelos gerados no BQML (ARIMA, TimesFM).

## Fluxo Principal

1. **Extração de dados** - BigQuery
2. **Limpeza e imputação** - Tratamento de dados faltantes
3. **Engenharia de features** - Lags e transformações exógenas
4. **Otimização de hiperparâmetros** - Optuna com validação cruzada
5. **Previsão** - Geração de projeções para próximos meses
6. **Avaliação** - MAPE dos modelos
7. **Exportação** - Resultados para BigQuery


## Saídas

As projeções são salvas em:
- `projecoes_modelos_sop_por_canal`
- `erros_modelos_sop_por_canal`
- `projecoes_melhores_modelos_sop_por_canal`

---
**Autores:** Ruan Sardi / Paulo Musachio

**Área:** Analytics
