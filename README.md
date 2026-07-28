# Guia de Estudos e Caderno Virtual de Análise de Dados no NotebookLM

[![NotebookLM](https://img.shields.io/badge/Acessar-NotebookLM-blue?style=for-the-badge&logo=google&logoColor=white)](COLE_O_SEU_LINK_AQUI)

> Miniguia prático, curadoria de fontes e documentação de engenharia de prompts sobre Análise de Dados, desenvolvido como projeto prático para a plataforma **DIO (Digital Innovation One)**.
> 
> 🔗 **Caderno Virtual:** [Clique aqui para abrir o projeto no Google NotebookLM](COLE_O_SEU_LINK_AQUI)

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

## Curadoria de Fontes Selecionadas por Tópico

Para alimentar o NotebookLM com materiais confiáveis e abertos, foram selecionadas 21 fontes abertas de alta autoridade técnica, divididas entre cada eixo temático do projeto. Abaixo foram citadas 5 fontes principais, uma para cada eixo:

### 1. Teoria, Fundamentos e Metodologia de Trabalho
Detalha o ciclo de vida clássico de projetos analíticos, abordando desde o entendimento do problema de negócio até a validação e implantação dos modelos.
* **Link:** [CRISP-DM Process Overview (Wikipedia)](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining)

---

### 2. Manipulação com Planilhas (Excel e Google Sheets)
Apresenta a estrutura conceitual de planilhas eletrônicas, lógica de fórmulas, referências cruzadas de células e agrupamentos por tabelas dinâmicas.
* **Link:** [Spreadsheets & Functions (Wikipedia)](https://en.wikipedia.org/wiki/Spreadsheet)

---

### 3. Consulta e Estruturação de Dados com SQL
Guia focado na prática analítica com SQL, ensinando desde filtragens e agregações até *Window Functions* para consultas temporais e agrupadas.
* **Link:** [PostgreSQL for Data Analysis Guide (Domo)](https://www.domo.com/learn/article/postgresql-for-data-analysis-a-complete-guide)

---

### 4. Visualização de Dados e Dashboards
Documentação oficial que ensina a estruturar dados no formato *Star Schema* (Fato e Dimensão) e criar métricas otimizadas para dashboards interativos.
* **Link:** [Power BI Data Modeling & DAX (Microsoft Learn)](https://learn.microsoft.com/pt-br/power-bi/transform-model/desktop-modeling-view)

---

### 5. IA Aplicada para Acelerar a Análise de Dados
Aborda os fundamentos e o funcionamento da Inteligência Artificial Generativa no suporte ao processamento de dados, automação de sintaxe e análise preditiva.
* **Link:** [Generative AI Overview (Wikipedia)](https://en.wikipedia.org/wiki/Generative_artificial_intelligence)

---

## Engenharia de Prompts e Registro de "Cicatrizes" (Troubleshooting)

Nesta seção estão documentados os testes realizados no NotebookLM, o raciocínio por trás dos prompts, os resultados, as referências utilizadas pela IA e a análise crítica das limitações observadas.

### Prompts Submetidos e Respostas Obtidas

#### Prompt 1: O Papel da IA Generativa na Análise
> **Pergunta:** *"De acordo com as fontes, como a IA generativa (ex: Copilot, Gemini) pode ser usada para auxiliar na escrita de consultas SQL e fórmulas DAX no Power BI sem substituir o pensamento crítico do analista?"*
>
> **Resultado da IA:** O NotebookLM entregou uma excelente resposta conceitual. Destacou a geração de DAX no Power BI e SQL no BigQuery, apontou o risco de alucinação e reforçou que a IA atua como ferramenta de aumento de produtividade, cabendo ao analista a validação do contexto do negócio.
>
> **Fontes Referenciadas no NotebookLM:** *Power BI Data Modeling & DAX (Microsoft Learn)* e *Generative AI Overview (Wikipedia)*.

#### Prompt 2: Ciclos de Vida, SQL Prático e Conexões no Power BI
> **Pergunta:** *"Com base nas fontes, explique as etapas do CRISP-DM, crie um guia comparando WHERE vs. HAVING com exemplo de ROW_NUMBER, e explique como conectar o Power BI ao SQL/Excel em um Star Schema."*
>
> **Resultado da IA:** O modelo priorizou a discussão sobre IA e omitiu o detalhamento das etapas do CRISP-DM e a sintaxe prática em código do SQL.
>
> **Fontes Referenciadas no NotebookLM:** *Generative AI Overview (Wikipedia)* (omitiu citações diretas das fontes de SQL e CRISP-DM devido à compressão do prompt).

### Registro de "Cicatrizes" (Limitações & Resolução de Problemas)

1. **Compressão do Contexto por Prompt Agrupado:**
   * **Dificuldade:** Ao enviar múltiplos tópicos complexos (CRISP-DM + SQL + Power BI + IA) em uma única mensagem, o modelo tendeu a responder com profundidade apenas o último tópico e generalizar/omitir os primeiros.
   * **Solução:** Fracionar as perguntas no NotebookLM em prompts individuais focados por tema.

2. **Aversão a Código Prático Formatado:**
   * **Dificuldade:** A IA respondeu em prosa fluida, ignorando a solicitação de exemplos em blocos de código SQL legíveis.
   * **Solução:** Adicionar restrições explícitas de formato no prompt, como: *"Forneça a resposta estruturada em Markdown, usando blocos de código SQL (` ```sql `) para demonstrar a sintaxe"*.

---

## Miniguia de Estudos

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

### 3. Conjunto de Prompts Reutilizáveis (Para Estudos Futuros)

Abaixo estão 3 templates de prompts testados e otimizados para reutilização no NotebookLM ou em outros assistentes de IA:

#### Prompt 1: Explicação de Código SQL
```text
Atue como um Analista de Dados Sênior. Com base nas fontes, explique a diferença conceitual e prática entre a cláusula WHERE e HAVING no SQL. Forneça um exemplo prático contendo um SELECT com GROUP BY e insira um bloco de código formatado.
```

#### Prompt 2: Modelagem Multidimensional no Power BI
```text
Com base no material de Business Intelligence, explique o que é o modelo Star Schema. Quais são as diferenças fundamentais entre uma tabela Fato e uma tabela Dimensão e como essa estrutura otimiza a performance de consultas e medidas DAX?
```

#### Prompt 3: Framework para Análise de Problemas de Negócio
```text
Atue como especialista em análise de negócios. Dado o ciclo de vida do CRISP-DM, descreva o passo a passo para mapear os requisitos da fase 'Entendimento do Negócio' antes de extrair qualquer dado do banco SQL. Liste 3 perguntas essenciais que o analista deve fazer aos stakeholders.
```

