# Caderno de Estudos e Guia Prático de Análise de Dados no NotebookLM

[![NotebookLM](https://img.shields.io/badge/Acessar-NotebookLM-blue?style=for-the-badge&logo=google&logoColor=white)](COLE_O_SEU_LINK_AQUI)

> Este repositório reúne um miniguia prático, curadoria de fontes de alta autoridade e a documentação de engenharia de prompts aplicada à área de Análise de Dados. O projeto foi desenvolvido como um laboratório prático para a **DIO (Digital Innovation One)**, explorando o uso da Inteligência Artificial Generativa como ferramenta de aprendizagem ativa.
> 
> 🔗 **Acesso ao Caderno Virtual:** [Clique aqui para abrir o projeto no Google NotebookLM](COLE_O_SEU_LINK_AQUI)

---

## Contexto e Objetivos

O propósito deste projeto é a construção de um **Caderno Temático no NotebookLM** focado no ecossistema de **Análise de Dados**. A proposta central é integrar o pensamento crítico do analista ao uso de IA Generativa, permitindo consolidar conceitos fundamentais, explorar ferramentas essenciais de mercado e compreender a integração com assistentes virtuais — **sem invadir escopos avançados de Engenharia de Dados ou Ciência de Dados pura (Machine Learning/MLOps)**.

### Objetivos Específicos:
* **Consolidar os fundamentos:** Compreender os ciclos de vida analíticos (CRISP-DM e metodologia Google) e a aplicação da estatística descritiva na resolução de problemas de negócios.
* **Mapear ferramentas essenciais:** Identificar o papel prático de planilhas eletrônicas (Excel/Sheets), linguagem de consulta (SQL) e plataformas de Business Intelligence (Power BI, Tableau e Looker).
* **Explorar o uso da IA como assistente:** Avaliar como assistentes generativos (Copilot, Gemini) otimizam a produtividade no ecossistema de dados, mantendo sempre a supervisão e validação humana.
* **Documentar o processo de IA ("cicatrizes"):** Registrar testes de prompts, refinamentos e as limitações encontradas durante o uso do NotebookLM.

---

## Curadoria de Fontes Selecionadas por Tópico

Para garantir que o NotebookLM trabalhasse apenas com conteúdos confiáveis, foram reunidas 21 fontes abertas de alta autoridade técnica, distribuídas entre os eixos do projeto. Abaixo estão destacadas as 5 fontes principais, representando cada tema estudado:

### 1. Teoria, Fundamentos e Metodologia de Trabalho
Detalha o ciclo de vida clássico de projetos analíticos, abordando desde o entendimento do problema de negócio até a validação e entrega final dos resultados.
* **Fonte principal:** [CRISP-DM Process Overview (Wikipedia)](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining)

---

### 2. Manipulação com Planilhas (Excel e Google Sheets)
Apresenta a estrutura conceitual das planilhas eletrônicas, a lógica de fórmulas, referências cruzadas de células e a consolidação de dados por tabelas dinâmicas.
* **Fonte principal:** [Spreadsheets & Functions (Wikipedia)](https://en.wikipedia.org/wiki/Spreadsheet)

---

### 3. Consulta e Estruturação de Dados com SQL
Guia focado na prática analítica com SQL, cobrindo desde filtragens e agregações básicas até o uso de *Window Functions* para consultas temporais e agrupadas.
* **Fonte principal:** [PostgreSQL for Data Analysis Guide (Domo)](https://www.domo.com/learn/article/postgresql-for-data-analysis-a-complete-guide)

---

### 4. Visualização de Dados e Dashboards
Documentação oficial focada na modelagem multidimensional em formato *Star Schema* (separação entre tabelas Fato e Dimensão) e na criação de métricas calculadas via DAX.
* **Fonte principal:** [Power BI Data Modeling & DAX (Microsoft Learn)](https://learn.microsoft.com/pt-br/power-bi/transform-model/desktop-modeling-view)

---

### 5. IA Aplicada para Acelerar a Análise de Dados
Aborda os fundamentos da Inteligência Artificial Generativa e sua aplicação prática na automação de sintaxes, suporte ao processamento de dados e análise preditiva.
* **Fonte principal:** [Generative AI Overview (Wikipedia)](https://en.wikipedia.org/wiki/Generative_artificial_intelligence)

---

## Engenharia de Prompts e Registro de "Cicatrizes" (Troubleshooting)

Esta seção documenta as consultas submetidas ao NotebookLM, o raciocínio por trás de cada prompt, os resultados gerados, as fontes utilizadas e a análise crítica das limitações observadas no processo.

### Prompts Submetidos e Respostas Obtidas

#### Prompt 1: O Papel da IA Generativa na Análise
> **Pergunta:** *"De acordo com as fontes, como a IA generativa (ex: Copilot, Gemini) pode ser usada para auxiliar na escrita de consultas SQL e fórmulas DAX no Power BI sem substituir o pensamento crítico do analista?"*
>
> **Resultado da IA:** O NotebookLM entregou uma resposta conceitual sólida. Destacou a geração de DAX no Power BI e SQL no BigQuery, alertou sobre o risco de alucinações e reforçou que a IA atua como ferramenta de produtividade, cabendo ao analista a validação do contexto do negócio.
>
> **Fontes citadas pela IA:** *Power BI Data Modeling & DAX (Microsoft Learn)* e *Generative AI Overview (Wikipedia)*.

#### Prompt 2: Ciclos de Vida, SQL Prático e Conexões no Power BI
> **Pergunta:** *"Com base nas fontes, explique as etapas do CRISP-DM, crie um guia comparando WHERE vs. HAVING com exemplo de ROW_NUMBER, e explique como conectar o Power BI ao SQL/Excel em um Star Schema."*
>
> **Resultado da IA:** O modelo priorizou a discussão sobre IA e omitiu o detalhamento das etapas do CRISP-DM, bem como a sintaxe prática em código SQL solicitada.
>
> **Fontes citadas pela IA:** *Generative AI Overview (Wikipedia)* (omitiu as fontes de SQL e CRISP-DM devido à sobrecarga de tópicos no prompt).

---

### Registro de "Cicatrizes" (Análise de Limitações)

1. **Compressão do Contexto por Prompt Agrupado:**
   * **Problema:** Ao enviar múltiplos tópicos complexos (CRISP-DM + SQL + Power BI + IA) em uma única mensagem, o modelo tendeu a focar no último assunto e generalizar os demais.
   * **Solução:** Fracionar as consultas no NotebookLM em prompts individuais e focados por tema.

2. **Aversão à Formatação de Código:**
   * **Problema:** A IA respondeu em texto corrido, ignorando a solicitação de exemplos práticos em blocos de código legíveis.
   * **Solução:** Adicionar restrições explícitas de formato no prompt, como: *"Forneça a resposta em formato Markdown, utilizando blocos de código SQL (` ```sql `)"*.

---

## Miniguia de Estudos

### 1. Resumos Estruturados do Assunto

#### A. O Ciclo de Vida da Análise (CRISP-DM & Google)
Projetos analíticos orientados ao valor começam no entendimento do problema, e não na tecnologia. O fluxo estruturado compreende:
1. **Entendimento do Negócio:** Mapear o problema e definir as perguntas estratégicas que precisam ser respondidas.
2. **Coleta e Preparação de Dados:** Extrair dados de bancos ou planilhas e realizar a limpeza (tratamento de duplicatas e valores nulos).
3. **Análise Exploratória:** Aplicar estatística descritiva (média, mediana, desvio padrão) para identificar padrões e anomalias.
4. **Visualização e Comunicação:** Traduzir dados em dashboards claros e focados nos KPIs estratégicos do negócio.
5. **Tomada de Ação:** Apresentar recomendações embasadas em dados para suportar as decisões gerenciais.

#### B. Ecossistema de Ferramentas
* **Planilhas (Excel/Sheets):** Indicadas para análises pontuais (*ad-hoc*), prototipagem rápida, limpeza básica e criação de relatórios com `VLOOKUP`, `XLOOKUP` e Tabelas Dinâmicas.
* **SQL (Queries):** Linguagem padrão para consultar e manipular grandes volumes de dados em bancos relacionais (PostgreSQL, MySQL, BigQuery). Permite aplicar filtros (`WHERE`), agrupamentos (`GROUP BY` / `HAVING`) e análises temporais via *Window Functions* (`ROW_NUMBER`).
* **Dashboards & BI (Power BI/Tableau/Looker):** Plataformas que conectam fontes heterogêneas, estruturam dados no modelo **Star Schema** (tabelas Fato conectadas a tabelas Dimensão) e publicam relatórios interativos.

---

### 2. Glossário de Conceitos Fundamentais

| Conceito | Definição Prática |
| :--- | :--- |
| **CRISP-DM** | *Cross-Industry Standard Process for Data Mining*. Metodologia padrão para condução de projetos analíticos. |
| **KPI** | *Key Performance Indicator*. Métrica quantitativa essencial para avaliar o atingimento dos objetivos de negócio. |
| **Star Schema** | Modelo de dados multidimensional composto por uma tabela Fato central conectada a tabelas Dimensão. |
| **DAX** | *Data Analysis Expressions*. Linguagem de fórmulas utilizada no Power BI para a criação de medidas e cálculos customizados. |

---

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

