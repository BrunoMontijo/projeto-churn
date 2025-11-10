📊 Análise Preditiva de Evasão de Clientes (Churn)

Status do Projeto: Concluído (Novembro/2025)

🎯 Objetivo do Projeto

O objetivo principal deste projeto é combater a evasão de clientes (Churn) em uma empresa de telecomunicações.

Utilizando técnicas de Ciência de Dados e Machine Learning, desenvolvemos um modelo preditivo capaz de identificar, com antecedência, quais clientes possuem maior risco de cancelar seus serviços, permitindo ações proativas de retenção.

📂 Dataset

Origem dos Dados: Plataforma Kaggle
Nome: Telco Customer Churn
Link para Download: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

🛠️ Tecnologias Utilizadas

Linguagem: Python 3

Bibliotecas: Pandas, Matplotlib, Seaborn, Scikit-Learn

Ambiente: Google Colab

🔍 Análise Exploratória (Principais Insights)

Durante a exploração dos dados, identificamos três fatores críticos que impulsionam o cancelamento:

Tipo de Contrato: Clientes com contratos mensais (Month-to-month) têm uma taxa de evasão drasticamente maior do que aqueles com contratos anuais.

Fatura Mensal: Existe uma correlação direta entre faturas mais altas e maior risco de evasão.

Tempo de Casa (Tenure): O risco é significativamente maior nos primeiros meses de relacionamento com o cliente.

🤖 Modelagem e Resultados

🤖 Modelagem e Resultados

Testamos três algoritmos diferentes utilizando Validação Cruzada (k=5) para garantir resultados robustos:

| Modelo                        | Acurácia Média |
| ----------------------------- | -------------- |
| Árvore de Decisão (Otimizada) | 78.75%         |
| Regressão Logística 🏆        | **80.35%**     |
| Random Forest                 | 79.10%         |

O modelo de Regressão Logística foi o campeão, apresentando a melhor performance geral.

📈 Desempenho do Modelo Campeão

Nosso modelo final é capaz de identificar corretamente mais da metade (Recall ≈ 52%) de todos os clientes que realmente iriam cancelar, com uma precisão de 62% nos alertas gerados.

🚀 Produto Final: A Lista de Risco

O resultado prático deste projeto é uma lista priorizada de clientes em risco.
Abaixo, um exemplo dos clientes com maior probabilidade de evasão identificados pelo modelo:

| ID do Cliente | Probabilidade de Churn (%) | Status Real    |
| ------------- | -------------------------- | -------------- |
| Cliente A     | 85.0%                      | Cancelou (Sim) |
| Cliente B     | 84.6%                      | Cancelou (Sim) |
| Cliente C     | 84.5%                      | Ativo (Não)    |

⚠️ Nota: O Cliente C, apesar de ainda estar ativo, foi identificado com altíssimo risco (84.5%) e deve ser priorizado para ações de retenção.

✒️ Autor

Bruno de Jesus Montijo
