# Data Pipeline e Recomendação com Filtragem Colaborativa

Este projeto implementa um **pipeline de ingestão e processamento de dados**, um **modelo de recomendação** baseado em **filtragem colaborativa**, e várias outras funcionalidades, como **monitoramento em tempo real** com Kafka, **geração de relatórios de performance**, e **análise de resultados de testes A/B**.

## Funcionalidades

### 1. Pipeline de Ingestão e Processamento de Dados
- Implementação de um pipeline de dados com **Apache Spark** para processar e armazenar dados provenientes do **Apache Kafka** em um data lake.
- Exemplo de uso de **Parquet** para armazenamento e checkpoints para garantir a resiliência do sistema.

### 2. Algoritmo de Filtragem Colaborativa
- Utiliza o **SVD** (Singular Value Decomposition) para realizar recomendações personalizadas para usuários com base em dados de interação.
- Implementação de **validação cruzada** para medir a performance do modelo usando métricas como RMSE e MAE.

### 3. API para Integração com a Plataforma
- Criação de uma **API REST** com **FastAPI** para expor o sistema de recomendação.
- A API permite que usuários solicitem recomendações com base no modelo previamente treinado.

### 4. Otimização do Pipeline de Dados
- Otimização da leitura e processamento de dados utilizando **caching** e configuração de **partições** no Spark para melhorar a performance.

### 5. Validação do Modelo de Recomendação
- Implementação de validação cruzada manual usando **KFold** para avaliar a performance do modelo de recomendação com maior detalhamento.

### 6. Geração de Relatórios de Performance do Pipeline
- Geração de relatórios de performance de execução de um pipeline Spark, com cálculos de tempo médio de execução por etapa.

### 7. Implementação de Métrica Customizada para o Modelo
- Criação de uma métrica customizada, o **Mean Percentage Error (MPE)**, para complementar as métricas tradicionais de RMSE e MAE na avaliação do modelo de recomendação.

### 8. Análise de Resultados dos Testes A/B
- Análise estatística dos resultados de um teste A/B, incluindo cálculo da taxa de cliques e comparação entre grupos de controle e de teste.

### 9. Monitoramento em Tempo Real com Apache Kafka
- Simulação de monitoramento de eventos de usuários em tempo real utilizando **Apache Kafka**.

### 10. Simulação de Cenários com o Modelo de Recomendação
- Simulação de diferentes cenários de recomendação utilizando o modelo treinado, fornecendo as melhores recomendações para um usuário específico.

## Como Executar

### Pré-requisitos
- **Python 3.x**
- **Apache Spark**
- **Apache Kafka**
- **FastAPI**
- **Surprise (para Filtragem Colaborativa)**

### Instalação

pip install -r requirements.txt
