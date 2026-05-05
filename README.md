# Miniguia de Estudos: Transição para Engenharia de Dados com NotebookLM
1. Contexto e Objetivos
Este projeto documenta o uso do NotebookLM para organizar o conhecimento necessário na transição de carreira de Analista de Dados para Engenheiro de Dados.

Assunto de Interesse: Arquiteturas de Dados Modernas (Medallion Architecture) e Processamento Distribuído com PySpark.

**Objetivos:**

Consolidar conceitos de limpeza e transformação de dados em camadas (Bronze, Silver, Gold).

Criar um fluxo de estudo otimizado para ferramentas como Microsoft Fabric e PySpark, que já fazem parte do meu ecossistema de aprendizado.

**2. Curadoria de Fontes**
Para alimentar o NotebookLM, selecionei as seguintes fontes técnicas:

Documentação Oficial do Microsoft Fabric: Foco em OneLake e Data Factory.

Guia de Melhores Práticas do PySpark: Foco em otimização de queries e processamento em larga escala.

Artigo sobre Arquitetura Medallion: Definições conceituais de organização de Data Lakes.

Material de Pós-graduação em Data Science: Notas de aula sobre Engenharia de Software e Banco de Dados.

**3. Engenharia de Prompts e "Cicatrizes"**
Nesta etapa, documentei como interagi com a IA para extrair o melhor conhecimento:

Prompt Estratégico 1: "Com base nos PDFs carregados, explique como a função broadcast no PySpark pode otimizar o join entre uma tabela de dimensões pequena e uma tabela de fatos grande."

Resultado: A IA inicialmente deu uma resposta genérica. Precisei ajustar o prompt para: "Explique o impacto técnico na memória do cluster ao usar broadcast join.".

Dificuldades (Troubleshooting): Identifiquei que o NotebookLM por vezes confundia termos de SQL tradicional com Spark SQL. A solução foi reforçar no prompt a necessidade de focar em "contexto de processamento distribuído".

**4. Miniguia de Estudo (Entrega Final)**
Resumo Estruturado: Arquitetura Medallion
Camada Bronze: Dados crus (Raw), sem transformações, servindo como histórico imutável.

Camada Silver: Dados limpos, filtrados e padronizados. É onde ocorre a maior parte do trabalho de Engenharia de Dados.

Camada Gold: Dados agregados e prontos para consumo por ferramentas de BI, como o Power BI.

Glossário de Conceitos-Chave
PySpark: Interface em Python para o Apache Spark, utilizada para processamento de Big Data.

OneLake: Conceito de "OneDrive para dados" dentro do Microsoft Fabric, unificando o armazenamento.

Data Activator: Ferramenta para automação de ações baseadas em padrões de dados.

Prompts Reutilizáveis para Revisão
"Resuma as principais diferenças entre um Data Lake e um Data Warehouse conforme os documentos fornecidos."

"Crie um quiz de 5 perguntas sobre otimização de scripts PySpark baseando-se no capítulo 3 do guia técnico."
