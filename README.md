# 🔥 DataForge Pipeline

[![Build Status](https://img.shields.io/github/actions/workflow/status/<usuario>/core-dataforge-pipeline-python/build.yml?branch=main)](https://github.com/<usuario>/core-dataforge-pipeline-python/actions)
[![Coverage](https://img.shields.io/codecov/c/github/<usuario>/core-dataforge-pipeline-python)](https://codecov.io/gh/<usuario>/core-dataforge-pipeline-python)
[![License](https://img.shields.io/github/license/<usuario>/core-dataforge-pipeline-python)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.12-blue)](https://www.python.org/)

---

## 🚀 Overview

**DataForge Pipeline** é um **framework robusto de ETL e processamento de dados** em Python, projetado para:

- Extrair, transformar e carregar dados de múltiplas fontes (SQL, NoSQL, APIs)  
- Orquestrar pipelines modulares, escaláveis e observáveis  
- Integrar com **EventHubX, CoreVault e TraceMatrix**  
- Suportar **paralelismo e processamento assíncrono**  
- Facilitar **auditoria, logging e monitoramento**  

Ideal para **data engineering, analytics e pipelines de dados críticos em produção**.

---

## 🏗 Architecture

```mermaid
graph TD
    Sources[SQL_NoSQL_APIs] -->|Extract| DataForge[Pipeline_Engine]
    DataForge -->|Transform| Tasks[Processing_Tasks_Python]
    DataForge -->|Load| Destinations[Data_Warehouse_DB_Files]
    DataForge -->|Event_Logs| EventHubX[EventHubX_GoBridge]
    DataForge -->|Observability| TraceMatrix[TraceMatrix_Prometheus_Grafana]
    DataForge -->|Secrets_Config| CoreVault[CoreVault]

