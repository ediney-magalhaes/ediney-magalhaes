# Olá, sou Ediney Magalhães 👋

Data & Analytics Engineer com formação em Estatística e mais de **10 anos de experiência estruturando ambientes analíticos em cenários reais de negócio**.

Especialista em **Arquitetura de Dados em Cloud, Engenharia de Dados, Analytics Engineering e Machine Learning aplicado**, atuando na construção de plataformas analíticas confiáveis, escaláveis e governadas.

Atuação focada em:

• Engenharia de Dados e Data Platforms  
• Arquiteturas analíticas em Cloud (Data Lake / Data Warehouse)  
• Governança de dados e conformidade (LGPD)  
• Otimização de performance e custos (FinOps)  
• Machine Learning aplicado a problemas reais de negócio  

---

# 🛠️ Tech Stack

### Cloud & Data Platform

![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=for-the-badge&logo=googlebigquery&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

### Data Engineering

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-003B57?style=for-the-badge&logo=postgresql&logoColor=white)
![Polars](https://img.shields.io/badge/Polars-1F77B4?style=for-the-badge)

### Analytics & Machine Learning

![ScikitLearn](https://img.shields.io/badge/ScikitLearn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=for-the-badge)

### BI & Visualização

![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Looker Studio](https://img.shields.io/badge/Looker%20Studio-4285F4?style=for-the-badge)

---

# 🚀 Projetos em Destaque

## 🏥 Plataforma Analítica Híbrida de Auditoria de Prontuários

🔗 https://github.com/qualidadehsr-rgb/auditoria-de-prontuarios

Ecossistema completo de auditoria hospitalar corporativa (**App Web + API + dbt + Data Warehouse + BI**) unificando dados legados em lote e novas submissões em tempo real.

Arquitetura construída para resolver o *Wide Table Problem* (mais de **600 itens por prontuário**) e gargalos de concorrência que inviabilizavam a análise de dados na instituição.

**Principais Tecnologias e Componentes:**
* **API Node.js:** Ingestão *near-real-time* via payload JSON dinâmico (Ingestão Pura).
* **Pipeline Serverless:** Extração autônoma de dados legados via Python + GitHub Actions.
* **Transformação com dbt:** Motor central de regras de negócio, qualidade de dados (Data Contracts) e unificação via **Surrogate Keys (MD5)**.
* **Arquitetura Medallion:** Separação robusta no BigQuery (Bronze, Silver e Gold).
* **Modelagem EAV (Entity-Attribute-Value):** Verticalização escalável via *Unpivot* dinâmico.
* **Privacy by Design:** Mascaramento automatizado de dados sensíveis para conformidade **LGPD**.

**O Impacto no Negócio:**
* **FinOps & Performance:** Transferência de cálculos analíticos do BI para o BigQuery, resultando em uma redução confirmada de **40%** no tempo de carregamento do dashboard (de 15,8s para 9,5s).
* **Escalabilidade Histórica:** Processamento e padronização impecável de mais de **104.820 registros legados**.
* **Single Source of Truth:** Eliminação total de perda de dados por concorrência simultânea.

---

## 🏛️ Data Lake Analytics — Governo Federal

🔗 https://github.com/ediney-magalhaes/gov-datalake-analytics

Arquitetura de **Data Lake em Cloud** para ingestão e governança de dados públicos do Governo Federal.

Arquitetura baseada em **Modern Data Stack e Medallion Architecture**.

Principais características:

• Ingestão de APIs governamentais com **dlt**  
• Processamento in-memory com **Polars**  
• Armazenamento colunar **Parquet**  
• Pseudonimização LGPD in-flight (SHA-256)  
• Dual logging para observabilidade  
• Registry Pattern para orquestração de pipelines  

---

## 🧠 Sistema Preditivo de Classificação Hospitalar

🔗 https://github.com/ediney-magalhaes/predicao-classificacao-hospitalar

Pipeline de Machine Learning para classificação automática de internações hospitalares.

O sistema classifica automaticamente:

• Grupo Assistencial  
• Complexidade SUS  

Principais técnicas:

• LightGBM  
• Balanceamento de classes com SMOTE  
• Feature engineering semântico baseado em **CID-10**  
• Integração com BigQuery para histórico e treinamento  

Impacto:

Automação de processo manual de classificação hospitalar (**~40 dias → minutos**).

---

## 📊 Pipeline Analítico BigQuery — Auditoria Hospitalar

🔗 https://github.com/ediney-magalhaes/bigquery-data-pipeline-auditoria

Pipeline ELT para consolidação de auditorias hospitalares provenientes de múltiplas planilhas Google Sheets.

Arquitetura:

• External Tables no BigQuery  
• Views consolidadas multi-tenant  
• Padronização de schema e tipagem  
• Tratamento de datas com Apps Script  

Resultado:

Visualização unificada de auditorias hospitalares no **Looker Studio**.

---

## 🤖 Agente de Inteligência Assistencial

🔗 https://github.com/ediney-magalhaes/agente-inteligencia-assistencial

Sistema baseado em **IA Generativa** para geração automática de relatórios analíticos hospitalares.

Capacidades:

• Consolidação automática de indicadores  
• Geração de relatórios técnicos com LLMs  
• Integração com ambiente analítico em Cloud  

---

## 🦟 Dengue MT — Sistema Preditivo de Surtos

🔗 https://github.com/ediney-magalhaes/dengue-mt

Projeto acadêmico para previsão de surtos de dengue utilizando:

• Dados epidemiológicos  
• Dados climáticos  
• Sensoriamento remoto  
• Modelos de Machine Learning  

Objetivo:

Antecipar surtos com **2–4 semanas de antecedência**.

---

# 🎓 Formação Acadêmica

📊 Estatística — UFMT  

🤖 Inteligência Artificial e Ciência de Dados — IFMT (cursando)  

🌐 Pós-graduação em Internet das Coisas — IFRO (cursando)

---

## 📫 Contato

<div> 
<a href="https://www.linkedin.com/in/ediney-magalhaes-estatistica-ciencia-dados" target="_blank">
  <img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white">
</a> 
<a href="mailto:edy.estatistica@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white">
</a>
</div>

---

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=8F0D87&height=120&section=footer"/>

