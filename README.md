# Projeto: Sensor DB + Modelo ML (Fase 5) — Hermes Reply Challenge

## Estrutura do repositório
- sql/create_tables.sql --> script SQL para criar o schema (tabelas e índices)
- data/sensor_dataset_simulated.csv --> dataset simulado
- output/confusion_matrix.png, timeseries_anomalies.png, rf_anomaly_detector.joblib
- notebook/ (espaço reservado para notebook Jupyter)
- README.md

## Banco de Dados
- Entidades: plant, asset, sensor, sensor_reading, event, anomaly_label, sensor_meta.
- Normalização: separação de metadados de sensores de leituras; índices em (sensor_id, timestamp).
- Script de criação disponível em sql/create_tables.sql

## Machine Learning
- Tarefa: Classificação binária (normal vs anomaly)
- Modelo: RandomForestClassifier
- Dataset: sensor_dataset_simulated.csv (800 leituras por sensor, 3 sensores)
- Resultados: Accuracy, classificação e gráficos (ver output/)

## Como reproduzir
1. Executar o script SQL em Oracle ou PostgreSQL ajustando tipos se necessário.
2. Rodar o notebook em notebook/ para gerar dataset e treinar modelo.
3. Artefatos gerados em data/ e output/.
