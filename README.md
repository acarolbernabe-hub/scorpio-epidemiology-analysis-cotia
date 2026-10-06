# Portal Epidemiológico e Dashboard de Acidentes por Escorpiões em Cotia

## 📌 Visão Geral do Projeto
Esta sendo desenvolvido como um produto integrador focado em **Ações de Ciência, Tecnologia e Inovação aplicadas à Saúde Pública** (alinhado aos ODS 3 e 11). Consiste em um portal público e um pipeline de dados reprodutível para monitoramento, análise estatística e visualização de acidentes escorpiônicos no município de Cotia (SP) e cidades espelho.

A solução integra dados brutos de notificações epidemiológicas inspiradas no padrão do **SINAN/DATASUS** combinados a variáveis climáticas locais para subsidiar a tomada de decisão da Vigilância Ambiental e Epidemiológica.

## 📊 Arquitetura de Dados e Pipeline (ETL)
O projeto foi estruturado seguindo um ciclo iterativo de engenharia de dados dividido em sprints:
1. **Aquisição e Preparação:** Extração, limpeza de categorias e tratamento de campos ausentes/ignorados em bases de notificações de acidentes por animais peçonhentos utilizando **Python (Pandas e NumPy)**.
2. **Análise Exploratória:** Estruturação de métricas descritivas e indutivas para responder às principais perguntas de negócio da saúde pública local.
3. **Sustentação e Deploy:** Hospedagem da base de conhecimento via GitHub Pages (MkDocs) e do dashboard interativo via **Streamlit Community Cloud**.

## 🔍 Perguntas de Negócio Respondidas pelos Dados
* **Evolução Temporal e Incidência:** Análise histórica ano a ano e cálculo da taxa de incidência normalizada por 100 mil habitantes, permitindo um benchmarking justo com municípios vizinhos (Carapicuíba, Itapevi, Embu das Artes).
* **Análise de Sazonalidade Climática:** Correlação entre os picos de acidentes e as variáveis de precipitação total (mm), umidade relativa média e temperatura média (°C) para subsidiar alertas preditivos em meses quentes.
* **Logística de Saúde e Atendimento:** Mensuração do tempo decorrido entre o momento da picada e o atendimento médico (ex: '0 a 1h', '1 a 3h'), identificando possíveis gargalos geográficos de socorro.
* **Perfil Sociodemográfico e Clínico:** Mapeamento de vulnerabilidades cruzando Faixa Etária, Sexo, Ocupação (trabalho rural/jardinagem) e gravidade clínica do caso para direcionamento de soroterapia aplicada.

## 🛠️ Tecnologias Utilizadas
* **Python:** Pandas, NumPy e SciPy (Engenharia de dados e modelagem estatística).
* **Streamlit & Plotly:** Construção da interface visual e gráficos dinâmicos.
* **Git & GitHub Pages:** Governança de código, controle de versões (Changelog) e documentação.

---
*Projeto Integrador II desenvolvido por Ana Carolina Bernabé no Curso Superior de Tecnologia em Ciência de Dados na FATEC Cotia (2º Semestre de 2026).*
