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
    Sources[SQL / NoSQL / APIs] -->|Extract| DataForge[Pipeline Engine]
    DataForge -->|Transform| Tasks[Processing Tasks (Python)]
    DataForge -->|Load| Destinations[Data Warehouse / DB / Files]
    DataForge -->|Event & Logs| EventHubX[EventHubX / GoBridge]
    DataForge -->|Observability| TraceMatrix[TraceMatrix / Prometheus / Grafana]
    DataForge -->|Secrets & Config| CoreVault[CoreVault]
