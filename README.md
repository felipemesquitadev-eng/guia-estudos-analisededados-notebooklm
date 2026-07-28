# Guia de Estudos e Caderno Virtual de Análise de Dados no NotebookLM

> Miniguia prático, curadoria de fontes e documentação de engenharia de prompts sobre Análise de Dados, desenvolvido como projeto prático para a plataforma **DIO (Digital Innovation One)**.

---

## Contexto e Objetivos

Este repositório reúne a documentação, curadoria e estrutura de conhecimento utilizadas para a criação de um **Caderno Temático no NotebookLM**, focado na área de **Análise de Dados**. 

O objetivo principal é aliar o pensamento crítico à Inteligência Artificial Generativa como ferramenta de aprendizagem ativa, explorando conceitos fundamentais de análise, ferramentas essenciais de mercado e a integração com IA, **sem invadir escopos avançados de Engenharia de Dados ou Ciência de Dados pura (Machine Learning/MLOps)**.

### Objetivos Específicos:
* **Consolidar os fundamentos:** Compreender ciclos de vida (CRISP-DM, metodologia Google) e estatística descritiva aplicada a negócios.
* **Dominar ferramentas essenciais:** Mapear o uso de planilhas (Excel/Google Sheets), linguagem de consulta (SQL) e ferramentas de Business Intelligence (Power BI/Tableau/Looker).
* **Explorar o uso de IA:** Analisar como assistentes generativos (Copilot, Gemini) otimizam a produtividade no ecossistema de dados mantendo a supervisão humana.
* **Documentar o processo de IA:** Registrar testes de prompts, refinamentos e as limitações ("cicatrizes") encontradas no NotebookLM.

---

## Curadoria de Fontes (20 Fontes Selecionadas)

Para alimentar o NotebookLM com materiais confiáveis e abertos, foram selecionadas 20 fontes divididas em 5 eixos temáticos:

### I. Teoria, Fundamentos e Metodologia de Trabalho
1. **[CRISP-DM Process Overview (Wikipedia)](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining):** Visão geral do ciclo de vida clássico de projetos de dados.
2. **[Google Data Analytics Professional Cert](https://www.coursera.org/professional-certificates/google-data-analytics):** Referência das 6 etapas da metodologia Google (*Perguntar, Preparar, Processar, Analisar, Compartilhar e Agir*).
3. **[Estatística e Probabilidade (Khan Academy)](https://pt.khanacademy.org/math/statistics-probability):** Conceitos de média, mediana, desvio padrão e distribuições.
4. **[Key Performance Indicators (Wikipedia)](https://en.wikipedia.org/wiki/Performance_indicator):** Definições de KPIs, métricas de negócio e indicadores *lagging/leading*.

### II. Manipulação com Planilhas (Excel e Google Sheets)
5. **[Spreadsheets & Functions (Wikipedia)](https://en.wikipedia.org/wiki/Spreadsheet):** Fundamentos de planilhas eletrônicas, referências de células e fórmulas.
6. **[VLOOKUP & Data Lookup (Wikipedia)](https://en.wikipedia.org/wiki/VLOOKUP):** Lógica e funcionamento de funções de busca e relacionamento de dados.
7. **[Treinamento do Microsoft Excel (Suporte Oficial)](https://support.microsoft.com/pt-br/excel):** Tabelas dinâmicas, formatação condicional e Power Query.
8. **[Data Cleansing Concepts (Wikipedia)](https://en.wikipedia.org/wiki/Data_cleansing):** Técnicas e conceitos essenciais para higienização e tratamento de dados.

### III. Consulta e Estruturação de Dados com SQL
9. **[PostgreSQL Developer Tutorials (Crunchy Data)](https://www.crunchydata.com/developers/tutorials):** Tutoriais de sintaxe SQL (`SELECT`, `WHERE`, `GROUP BY`, `HAVING`).
10. **[PostgreSQL for Data Analysis Guide (Domo)](https://www.domo.com/learn/article/postgresql-for-data-analysis-a-complete-guide):** Uso avançado de *Window Functions* e subqueries em SQL.
11. **[BigQuery Documentation (Google Cloud)](https://cloud.google.com/bigquery/docs):** Consultas em nuvem e manipulação de grandes volumes de dados.
12. **[BigQuery Connected Sheets (Google Cloud)](https://cloud.google.com/bigquery/docs/connected-sheets):** Conexão direta entre bancos de dados SQL e planilhas.

### IV. Visualização de Dados e Dashboards
13. **[Power BI Data Connectivity (Microsoft Learn)](https://learn.microsoft.com/pt-br/power-bi/connect-data/):** Conectar fontes de dados (Excel, CSV e bancos SQL) no Power BI.
14. **[Power BI Data Modeling & DAX (Microsoft Learn)](https://learn.microsoft.com/pt-br/power-bi/transform-model/desktop-modeling-view):** Modelagem multidimensional (*Star Schema*) e criação de métricas DAX.
15. **[Tableau Public Tutorial](https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-build.htm):** Construção de relatórios e painéis interativos.
16. **[Google Looker Studio Documentation](https://support.google.com/looker-studio/):** Criação de dashboards em nuvem conectados ao Sheets e BigQuery.
17. **[Fundamentals of Data Visualization (Claus O. Wilke)](https://clauswilke.com/dataviz/):** Teoria das cores, escolha de gráficos e boas práticas de design/UX.

### V. IA Aplicada para Acelerar a Análise de Dados
18. **[Microsoft Copilot no Power BI](https://learn.microsoft.com/pt-br/power-bi/create-reports/copilot-introduction):** Uso de IA para geração de expressões DAX e resumos executivos.
19. **[OpenAI Cookbook (SQL Prompts)](https://cookbook.openai.com/):** Exemplos de engenharia de prompt para geração e depuração de queries SQL.
20. **[Generative AI Overview (Wikipedia)](https://en.wikipedia.org/wiki/Generative_artificial_intelligence):** Conceitos de IA generativa aplicada ao processamento e automação de análises.

---

## Engenharia de Prompts e Registro de "Cicatrizes" (Troubleshooting)

Nesta seção estão documentados os testes realizados no NotebookLM, o raciocínio por trás dos prompts e a análise crítica das limitações observadas.

### Prompts Submetidos e Respostas Obtidas

#### Prompt 1: O Papel da IA Generativa na Análise
> **Pergunta:** *"De acordo com as fontes, como a IA generativa (ex: Copilot, Gemini) pode ser usada para auxiliar na escrita de consultas SQL e fórmulas DAX no Power BI sem substituir o pensamento crítico do analista?"*
>
> **Resultado da IA:** O NotebookLM entregou uma excelente resposta conceitual. Destacou a geração de DAX no Power BI e SQL no BigQuery, apontou o risco de alucinação e reforçou que a IA atua como ferramenta de aumento de produtividade, cabendo ao analista a validação do contexto do negócio.

#### Prompt 2: Ciclos de Vida, SQL Prático e Conexões no Power BI
> **Pergunta:** *"Com base nas fontes, explique as etapas do CRISP-DM, crie um guia comparando WHERE vs. HAVING com exemplo de ROW_NUMBER, e explique como conectar o Power BI ao SQL/Excel em um Star Schema."*
>
> **Resultado da IA:** O modelo priorizou a discussão sobre IA e omitiu o detalhamento do CRISP-DM e a sintaxe prática em código do SQL.

### Registro de "Cicatrizes" (Limitações & Resolução de Problemas)

1. **Compressão do Contexto por Prompt Agrupado:**
   * **Dificuldade:** Ao enviar múltiplos tópicos complexos (CRISP-DM + SQL + Power BI + IA) em uma única mensagem, o modelo tendeu a responder com profundidade apenas o último tópico e generalizar os primeiros.
   * **Solução:** Fracionar as perguntas no NotebookLM em prompts individuais focados por tema.

2. **Aversão a Código Prático Formatado:**
   * **Dificuldade:** A IA respondeu em prosa fluida, ignorando a solicitação de exemplos em blocos de código SQL legíveis.
   * **Solução:** Adicionar restrições explícitas de formato no prompt, como: *"Forneça a resposta estruturada em Markdown, usando blocos de código SQL (` ```sql `) para demonstrar a sintaxe"*.

---

## Miniguia de Estudo (Entrega Final)

### 1. Resumos Estruturados do Assunto

#### A. O Ciclo de Vida da Análise (CRISP-DM & Google)
Toda análise de dados de sucesso começa no negócio, não nos dados. 
1. **Entendimento do Negócio:** Mapear o problema real e definir as perguntas que precisam ser respondidas.
2. **Coleta e Preparação de Dados:** Extrair de bancos de dados ou planilhas e realizar a limpeza (tratamento de duplicatas e nulos).
3. **Análise Exploratória:** Aplicar estatística descritiva (média, mediana, desvio padrão) para identificar padrões e anomalias.
4. **Visualização e Comunicação:** Traduzir dados em gráficos claros (dashboards) focados nos KPIs estratégicos.
5. **Tomada de Ação:** Apresentar *insights* recomendando decisões baseadas em evidências.

#### B. Ecossistema de Ferramentas
* **Planilhas (Excel/Sheets):** Ideais para ad-hoc analysis, prototipagem rápida, limpeza básica e relatórios pontuais com `VLOOKUP`, `XLOOKUP` e Tabelas Dinâmicas.
* **SQL (Queries):** A linguagem padrão para manipular e consultar volumes maiores em bancos relacionais (PostgreSQL, MySQL, BigQuery). Permite filtrar (`WHERE`), agregar (`GROUP BY` / `HAVING`) e realizar análises temporais com *Window Functions* (`ROW_NUMBER`).
* **Dashboards & BI (Power BI/Tableau/Looker):** Ferramentas para conectar fontes heterogêneas (Excel + SQL), modelar dados em **Star Schema** (Tabelas Fato de eventos ligadas a Tabelas Dimensão de contexto) e publicar relatórios interativos.

---

### 2. Glossário de Conceitos Fundamentais

| Conceito | Definição Prática |
| :--- | :--- |
| **CRISP-DM** | *Cross-Industry Standard Process for Data Mining*. Metodologia padrão para conduzir projetos analíticos. |
| **KPI** | *Key Performance Indicator*. Métrica quantitativa essencial para medir o sucesso de um objetivo de negócio. |
| **Star Schema** | Modelo de dados otimizado para BI com uma tabela Fato central cercada por tabelas Dimensão. |
| **DAX** | *Data Analysis Expressions*. Linguagem de fórmulas utilizada no Power BI para criar medidas calculadas. |
| **Window Function** | Função SQL (ex: `ROW_NUMBER()`, `RANK()`) que realiza cálculos através de um conjunto de linhas relativas à linha atual. |
| **Alucinação (IA)** | Fenômeno em que a IA generativa produz uma resposta incorreta ou inventada com tom de certeza. |

---

### 3. Conjunto de Prompts Reutilizáveis (Para Estudos Futuros)

Abaixo estão 3 templates de prompts testados e otimizados para reutilização no NotebookLM ou em outros assistentes de IA:

#### 🟢 Prompt para Explication de Código SQL:
```text
Atue como um Analista de Dados Sênior. Com base nas fontes, explique a diferença conceitual e prática entre a cláusula WHERE e HAVING no SQL. Forneça um exemplo prático contendo um SELECT com GROUP BY e insira um bloco de código formatado.
```
