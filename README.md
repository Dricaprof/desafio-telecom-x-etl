# 📊 Projeto Telecom X – Análise de Evasão de Clientes (ETL)

Este repositório contém a solução do desafio proposto no programa de formação em Data Science, com foco na aplicação prática do processo de **ETL – Extração, Transformação e Carga** de dados reais de negócios. O projeto utiliza os dados da empresa fictícia Telecom X, que enfrenta altos índices de **evasão de clientes (churn)**.

---

## 🎯 Propósito da Análise

O objetivo do projeto é:

- Praticar as etapas fundamentais de um processo de ETL com Python;
- Preparar os dados da empresa Telecom X para futuras análises e modelagens preditivas;
- Entregar um conjunto de dados limpo, estruturado e pronto para ser usado pela equipe de Data Science.

---

## 🗂️ Estrutura do Projeto

| Arquivo                  | Descrição                                                                 |
|--------------------------|---------------------------------------------------------------------------|
| `notebook_telecom_etl.ipynb` | Notebook com todo o processo de ETL e relatório explicativo em Markdown |
| `dados_tratados.csv`         | Base de dados final, limpa e estruturada para análise                   |
| `README.md`                  | Documentação do projeto                                                 |

---

## 📈 Exemplos de Gráficos e Insights

Durante a análise exploratória (opcional), alguns gráficos podem ser utilizados para entender o perfil dos clientes que evadem, por exemplo:

- **Distribuição de churn** (clientes que cancelam vs. permanecem)
- **Churn por tipo de contrato**
- **Relação entre tempo de contrato (`tenure`) e churn**
- **Churn por forma de pagamento**

Exemplo de gráfico:

```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.countplot(data=df_final, x='churn')
plt.title("Distribuição de Clientes com e sem Evasão")
plt.show()
