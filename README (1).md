# 📊 Challenge Telecom X – Análise de Evasão de Clientes  

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python" />
  <img src="https://img.shields.io/badge/Status-Concluído-brightgreen?style=flat-square" />
  <img src="https://img.shields.io/badge/Desafio-Data%20Science-orange?style=flat-square" />
</p>

---

## 🚀 Sobre o Desafio  

A **Telecom X** enfrenta um problema crítico: um alto índice de cancelamento de clientes (**churn**).  
O objetivo deste desafio foi **coletar, transformar, analisar e visualizar dados** para compreender os fatores que influenciam a evasão e gerar **insights estratégicos** para retenção de clientes.  

Este projeto é a **fase exploratória (EDA)**, mas serve como base para futuros **modelos preditivos de Machine Learning**.  

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas  

- 🐍 **Python 3.9+**  
- 📊 **Pandas** → manipulação de dados  
- 🌐 **Requests & JSON** → coleta de dados via API  
- 📈 **Matplotlib & Seaborn** → visualizações gráficas  
- 🔢 **NumPy** → operações numéricas  

---

## 📂 Estrutura do Projeto  

1. **📌 Extração**  
   - Dados obtidos de uma **API em JSON**.  
   - Importados e carregados no Pandas DataFrame.  

   ```python
   import pandas as pd
   import requests, json

   url = "https://raw.githubusercontent.com/ingridcristh/challenge2-data-science/main/TelecomX_Data.json"
   dados = pd.read_json(url)
   dados.head()
   ```

2. **🔧 Transformação**  
   - Normalização dos dados.  
   - Renomeação das colunas para nomes amigáveis em português.  

   ```python
   dados.rename(columns={
       "customerID": "ID_Cliente",
       "Churn": "Cancelamento",
       "customer/gender": "Gênero",
       "customer/SeniorCitizen": "Idoso",
       "account/Contract": "Tipo_Contrato",
       "account/PaymentMethod": "Forma_Pagamento",
       "account/Charges/Monthly": "Valor_Mensal",
   }, inplace=True)
   ```

3. **🔎 Análise Exploratória (EDA)**  
   - Análise do perfil de clientes (**idade, dependentes, tempo de contrato**).  
   - Comparação entre **clientes ativos e cancelados**.  
   - Estudo do impacto de **contratos, serviços e formas de pagamento**.  

4. **📈 Visualizações**  
   - Distribuição do churn.  
   - Relação entre **tempo de contrato e evasão**.  
   - Comparativo de **formas de pagamento**.  
   - Serviços adicionais x cancelamento.  

---

## 🔍 Principais Insights  

✅ **Contratos mensais** → maiores índices de churn.  
✅ **Clientes com fatura digital** cancelam mais do que os que recebem boleto.  
✅ **Serviços extras (TV, filmes, segurança online, backup)** ajudam na fidelização.  
✅ **Pagamentos automáticos** reduzem a evasão.  
✅ Quanto maior o **tempo de contrato**, maior a chance de permanência.  

---

## ✅ Conclusões  

📌 O cancelamento de clientes **não é aleatório**: fatores como contrato, forma de pagamento e serviços adicionais exercem grande influência.  

**Possíveis estratégias de retenção:**  
- Incentivar **contratos de longo prazo** com descontos.  
- Recompensar quem adota **serviços combinados**.  
- Melhorar a experiência de quem usa **fatura digital**.  
- Oferecer benefícios para quem **ativa débito automático**.  

➡️ Este projeto serviu como **ponto de partida**.  
A evolução natural é criar **modelos de Machine Learning** para prever clientes em risco de churn e agir **proativamente**.  

---

## 📊 Exemplo de Visualização  

<p align="center">
  <img src="https://github.com/matplotlib/matplotlib/raw/main/doc/_static/logo2_compressed.svg" alt="Exemplo de gráfico" width="200"/>
</p>

*(Exemplo ilustrativo – gráficos reais são gerados no notebook do projeto).*  

---

## 👩‍💻 Autor  

📌 Desafio desenvolvido no notebook **`Challenge_TelecomX.ipynb`**.  
💡 Sinta-se à vontade para contribuir, sugerir melhorias ou implementar modelos preditivos! 🚀  

---
