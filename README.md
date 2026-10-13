# Olá, sou Ediney Magalhães 👋

Estatístico e cientista de dados com mais de 10 anos de experiência em dados. Uso engenharia de dados para entregar ciência de dados que funciona no negócio: modelos preditivos e análises em produção, sobre plataformas em nuvem (GCP) confiáveis e governadas.

Meu foco é transformar dados em decisão: previsão com validação rigorosa, indicadores confiáveis e comunicação clara com áreas não técnicas.

Atuação focada em:
- Ciência de dados: Machine Learning, previsão (séries temporais) e estatística aplicada
- Analytics e BI: indicadores, dashboards e métricas de negócio (Power BI, Looker Studio)
- Engenharia de dados aplicada: pipelines, Data Lake / Data Warehouse e MLOps em Cloud
- Governança de dados e conformidade (LGPD)
- Otimização de performance e custos (FinOps) 

---

# 🛠️ Tech Stack

### Ciência de Dados e Machine Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![ScikitLearn](https://img.shields.io/badge/ScikitLearn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=for-the-badge)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)

### Analytics e BI

![SQL](https://img.shields.io/badge/SQL-003B57?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Looker Studio](https://img.shields.io/badge/Looker%20Studio-4285F4?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

### Engenharia de Dados

![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=for-the-badge&logo=googlebigquery&logoColor=white)
![Polars](https://img.shields.io/badge/Polars-1F77B4?style=for-the-badge)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black)
![Dagster](https://img.shields.io/badge/Dagster-4F43DD?style=for-the-badge&logo=dagster&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)

### Cloud e Automação

![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

# 🚀 Projetos em Destaque

## 🦟 Dengue MT — Previsão de Surtos com Machine Learning

🔗 https://github.com/ediney-magalhaes/dengue-mt

Projeto acadêmico (IFMT) de ponta a ponta, da ingestão de dados públicos ao modelo e ao dashboard em produção, para antecipar surtos de dengue em Cuiabá e Várzea Grande, com horizonte de 1 a 8 semanas.

Modelo e validação
• LightGBM com validação temporal (TimeSeriesSplit, 5 folds): R² de 0,741 ± 0,081 e erro médio de 9,7 casos por semana
• Intervalos de predição (CQR) com cobertura empírica de 91,5% para o nível de 90%
• Interpretabilidade com SHAP

Engenharia a serviço do modelo
• 5 fontes públicas integradas (InfoDengue, NASA POWER, NOAA, MODIS e Google Trends) em arquitetura medalhão, com dbt e DuckDB
• Rastreio de experimentos com MLflow, orquestração com Prefect e dashboard em Streamlit

---

## 🧠 Classificação Hospitalar SUS — Machine Learning em Produção

🔗 https://github.com/ediney-magalhaes/predicao-classificacao-hospitalar

Sistema em produção que classifica internações hospitalares em Grupo Assistencial (clínico, cirúrgico, diagnóstico, OPME) e Complexidade (básica, média, alta), usado na elaboração de perfil e na auditoria. Substituiu a leitura manual de cerca de 900 prontuários por mês, que consumia cerca de 40 dias de trabalho, por um processamento em menos de 1 minuto, operado por uma assistente não técnica em interface web na rede do hospital.

Modelo e evolução
• LightGBM com SMOTE e variáveis derivadas da CID-10 (capítulo e grupo), treinado sobre mais de 110 mil registros (2012–2026)
• Acurácia de cerca de 95–96% nos dois alvos
• Evolução da v1 à v5: recall em alta complexidade de 56% para 89%; F1 do Grupo SUS de 0,63 para 0,87
• Score de confiança por predição (abaixo de 70% é sinalizado para revisão) e regra de negócio que corrige automaticamente casos clínicos com cirurgia registrada

Engenharia e analytics
• Validação dos dados de entrada com Pandera e ciclo de correção humana que realimenta o modelo
• Camada analítica em dbt (staging, intermediate e marts de volume assistencial, taxa de correção e passagem por UTI), com dashboards de BI em construção
• Anonimização SHA-256 com salt antes do envio à nuvem; os dados de internação não trafegam pela internet pública
• Custo de infraestrutura de R$ 0 por mês; ADRs, model cards e runbooks documentados

---

## 🏥 Auditoria Clínica de Prontuários — Dados e BI para 9 Unidades

🔗 https://github.com/ediney-magalhaes/auditoria-de-prontuarios

Plataforma de ponta a ponta (app web, API, dbt, Data Warehouse e BI) que automatiza a auditoria clínica de prontuários de 9 unidades hospitalares e transforma as avaliações em indicadores de conformidade para a gestão.

Analytics e impacto
• Taxa de Conformidade (itens conformes sobre itens válidos) com cortes por unidade, setor, tipo de prontuário, especialidade, avaliador e período, em dashboards no Looker Studio
• Dashboard 76% mais rápido (de 11,8 s para 2,8 s) e relatório consolidado de 24 para 5 páginas
• Mais de 104 mil registros históricos unificados em uma única fonte da verdade

Engenharia
• Ingestão em tempo quase real via API Node.js e carga histórica via Python e GitHub Actions
• Arquitetura medalhão no BigQuery, com regras de negócio e qualidade de dados em dbt
• Modelagem EAV com unpivot dinâmico para prontuários com mais de 600 itens
• Mascaramento automático de dados sensíveis (LGPD) na camada final

---

## 🤖 Agente de Inteligência Assistencial — IA Generativa para Relatórios

🔗 https://github.com/ediney-magalhaes/agente-inteligencia-assistencial

Sistema que automatiza o relatório trimestral de segurança do paciente, antes consolidado manualmente em cerca de 30 dias e hoje gerado em menos de 1 dia.

• Aplicação em Streamlit que processa 10 blocos analíticos, com gráficos e análises interpretativas geradas por LLM (Gemini API) sob demanda
• Engenharia de prompt para transformar os indicadores calculados em texto de análise
• Engenharia de software documentada: 17 ADRs, versionamento semântico com CHANGELOG, roadmap por fases e backlog
• Em evolução: revisão estruturada em andamento. Planejados, por fases: testes automatizados, base histórica, painel epidemiológico, um agente com busca semântica e RAG sobre o histórico de notificações

---

## 🏛️ Data Lake de Gestão de Pessoas — Governo Federal

🔗 https://github.com/ediney-magalhaes/gov-datalake-analytics

Projeto pessoal de plataforma analítica de ponta a ponta com dados públicos de pessoal do Executivo Federal (SIAPE, DEPRO e ENAP), estruturada para estudos de trajetória de carreira, remuneração, aposentadoria, competências e diversidade.

Escala e engenharia
• Mais de 276 milhões de registros ingeridos (2015 a 2026, 8 conjuntos de dados com 136 partições mensais cada), com 17,3 GB em Parquet particionado
• Orquestração com Dagster e ingestão em memória com Polars, a cerca de 14 mil registros por segundo; Google Cloud Storage com particionamento Hive e BigQuery como Data Warehouse
• Pseudonimização SHA-256 durante a ingestão (LGPD)

Modelagem analítica (dbt)
• Camada Silver concluída, com 8 modelos de staging e 48 testes de qualidade
• Camada Gold em finalização: modelagem dimensional (Kimball) com 8 fatos e 7 dimensões; os maiores fatos têm de 76 a 97 milhões de linhas
• Grão de cada fato validado em população completa, nunca por amostra, o que revelou duplicidades e colisões de identificador antes que chegassem às análises
• Arquitetura medalhão documentada em ADRs, com termos de homologação por camada  

---

## 📊 Pipeline Analítico no BigQuery — Auditoria de Conformidade em 5 Unidades

🔗 https://github.com/ediney-magalhaes/bigquery-data-pipeline-auditoria

Pipeline ELT que consolida em um único painel as auditorias de conformidade de 5 unidades hospitalares, antes registradas em planilhas Google Sheets separadas.

• External Tables no BigQuery lendo diretamente das planilhas de cada unidade
• Views consolidadas multi-tenant, com padronização de schema e tipagem entre unidades
• Tratamento de datas automatizado com Google Apps Script
• Dashboard unificado no Looker Studio  

Resultado:

Visualização unificada de auditorias hospitalares no **Looker Studio**.

---

## 🎓 Formação e Publicações

**Formação**
- Graduação em Estatística, UFMT (concluída em 2024)
- Pós-graduação em IoT, IFRO (concluída em julho de 2026)
- Graduação em IA e Ciência de Dados, IFMT (em andamento)

**Trabalhos apresentados em congressos**
- **CBIS 2026:** Sistema Preditivo de Dengue Baseado em Machine Learning para Apoio à Vigilância Epidemiológica Municipal
- **CONAHP 2025:** IA Estratégica na Gestão Hospitalar: Previsão de Custo e Otimização de Recursos
- **CONAHP 2023:** Uso de métodos estatísticos para previsão da taxa de ocupação hospitalar

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

