# Challenge Telecom x PT1

Este projeto apresenta uma análise detalhada da evasão de clientes (**churn**) da empresa fictícia Telecom X, utilizando Python em um único notebook Jupyter: [`Challenge_TelecomX.ipynb`](Challenge_TelecomX.ipynb).

---

## 📊 Objetivo

O principal objetivo é identificar os fatores que levam ao cancelamento de clientes, usando técnicas de ciência de dados (ETL, EDA e visualização) para responder às principais perguntas do negócio e propor ações baseadas em evidências.

---

## 🛠️ Estrutura do Projeto

- **Arquivo Principal:** `Challenge_TelecomX.ipynb`
- **Fonte de Dados:** Importação de um dataset JSON hospedado externamente via API.
- **Principais Etapas:**
  1. **Extração:** Coleta dos dados via API, carregando-os em um DataFrame do pandas.
  2. **Transformação:** Normalização dos dados, tradução das colunas para o português, limpeza e organização.
  3. **Análise Exploratória (EDA):** Visualizações com matplotlib e seaborn, estatísticas e identificação de padrões de churn.
  4. **Relatório de Insights:** Geração de gráficos e recomendações para retenção de clientes.

---

## 💡 Destaques Técnicos

- **Bibliotecas Utilizadas:** `pandas`, `requests`, `json`, `matplotlib`, `seaborn`, `numpy`
- **Processo ETL:** Extração eficiente de dados da API, transformação detalhada (normalização e tradução), preparação para análise.
- **Visualização:** Diversos tipos de gráficos facilitam a compreensão dos padrões de cancelamento.
- **Tradução:** Todas as colunas são adaptadas para o português, tornando a análise mais acessível.

---

## 👀 Exemplos de Dados

O dataset contém informações como:
- ID do cliente
- Status de cancelamento (churn)
- Gênero, idade, dependentes
- Serviços contratados (telefone, internet, streaming, backup)
- Detalhes do contrato e método de pagamento
- Valores pagos

---

## 🚀 Como Executar

1. Clone o repositório:
   ```sh
   git clone https://github.com/Matheusisa/Challenge-Telecom-x-PT1.git
   ```
2. Abra o notebook `Challenge_TelecomX.ipynb` no Jupyter Notebook ou Google Colab.
3. Execute as células em ordem para realizar a análise.

---

## 📈 Resultados Esperados

- Identificação dos principais fatores de churn
- Insights sobre os perfis de clientes mais propensos ao cancelamento
- Recomendações para retenção com base nos dados
- Visualizações claras e objetivas para orientar decisões estratégicas

---

## 📝 Autor

Desenvolvido por [Matheusisa](https://github.com/Matheusisa).

---

## 📄 Licença

Licenciado sob a MIT License.

---

> **Este projeto é ideal para quem deseja aprender sobre ETL, EDA e análise de churn em telecomunicações, de forma prática e didática!**
