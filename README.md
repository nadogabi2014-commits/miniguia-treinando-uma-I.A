# 📘 Miniguia: Treinando uma I.A

Bem-vindo ao repositório **miniguia-treinando-uma-ia**. Este projeto documenta a criação, alimentação, engenharia de prompts e consolidação de conhecimentos utilizando o **Google NotebookLM**, uma ferramenta de inteligência artificial baseada no modelo Gemini, voltada para análise e síntese de fontes de informação confiáveis.

---

## 🎯 Contexto e Objetivos do Projeto

### Contexto
O ecossistema de Inteligência Artificial Generativa evoluiu do consumo passivo para a construção de assistentes fundamentados em dados próprios (Retrieval-Augmented Generation / RAG). O **NotebookLM** da Google destaca-se por permitir que o usuário crie um "caderno temático" alimentado exclusivamente por fontes selecionadas, garantindo respostas sem alucinações genéricas e focadas no material fornecido.

**Tema Escolhido para o Caderno Temático:** *Fundamentos e Boas Práticas de Engenharia de Prompts e Arquitetura de I.A Generativa*.

---

### Objetivos de Estudo
1. **Curadoria de Dados:** Selecionar e preparar documentos em texto/PDF de alta qualidade sobre IA.
2. **Experimentação Prática:** Testar a capacidade de síntese, cruzamento de dados e geração de insights do NotebookLM.
3. **Engenharia de Prompts com Foco em Fontes:** Desenvolver e refinar perguntas estratégicas para extrair análises precisas do material.
4. **Mapeamento de "Cicatrizes":** Registrar desafios, alucinações, limites da ferramenta e estratégias de contorno.
5. **Consolidação do Aprendizado:** Gerar resumos, glossários e um guia de prompts reutilizáveis.

---

## 📚 Curadoria de Fontes (Alimentação do NotebookLM)

Para alimentar o NotebookLM, foram selecionados **4 materiais de acesso aberto** sobre Inteligência Artificial, Engenharia de Prompts e RAG:

1. **[PDF] Prompt Engineering Guide (DAIR.AI)**
   * *Descrição:* Guia abrangente com conceitos avançados de engenharia de prompts (Chain-of-Thought, Few-Shot Prompting, ReAct).
   * *Link:* [https://www.promptingguide.ai/](https://www.promptingguide.ai/)

2. **[Artigo/PDF] A Survey on Retrieval-Augmented Generation (RAG)**
   * *Descrição:* Artigo acadêmico detalhando como a busca em fontes externas melhora as respostas dos modelos de linguagem.
   * *Link:* [https://arxiv.org/abs/2312.10997](https://arxiv.org/abs/2312.10997)

3. **[Documentação] Google AI Studio - Prompt Engineering Best Practices**
   * *Descrição:* Boas práticas oficiais da Google para escrita de prompts eficazes para a família Gemini.
   * *Link:* [https://ai.google.dev/gemini-api/docs/prompting-strategies](https://ai.google.dev/gemini-api/docs/prompting-strategies)

4. **[Relatório/Artigo] Ethics and Governance of Artificial Intelligence**
   * *Descrição:* Documento focado nos impactos, governança e viés em sistemas de IA.
   * *Link:* [https://www.unesco.org/en/artificial-intelligence/recommendation-ethics](https://www.unesco.org/en/artificial-intelligence/recommendation-ethics)

---

## 🛠️ Engenharia de Prompts e "Cicatrizes" (Aprendizados e Desafios)

Nesta seção são registradas as interações, variações de testes, dificuldades encontradas e o valor dessa competência no mercado.

### 1. Testes de Prompts e Variações

#### **Prompt 1 (Ingênuo / Direto)**
> *"O que o material diz sobre engenharia de prompts?"*
* **Resultado:** Resposta genérica e rasa, listando apenas definições básicas sem cruzar as fontes.
* **Citação do Material:** Citou superficialmente o Guia da DAIR.AI.

#### **Prompt 1 Refinado (Estratégico / Papel e Formato)**
> *"Atue como um Especialista em IA. Com base EXCLUSIVAMENTE nas fontes fornecidas, crie uma tabela comparativa entre Few-Shot Prompting e Chain-of-Thought Prompting, detalhando: 1) Definição, 2) Quando usar, e 3) Exemplo prático citado nos PDFs."*
* **Resultado:** Resposta altamente estruturada em tabela HTML/Markdown, citando exatamente as seções do PDF da DAIR.AI e do documento da Google.

---

### 2. "Cicatrizes" (Dificuldades e Limitações Encontradas)

| Desafio/Limitação Encontrada | Causa Identificada | Solução/Contorno Aplicado |
| :--- | :--- | :--- |
| **Respostas evasivas sobre comparações** | O NotebookLM tendia a resumir fonte por fonte em vez de sintetizar. | Forçar a estrutura no prompt (ex: *"Crie uma matriz de comparação única combinando as fontes A e B"*). |
| **Perda de detalhes técnicos em PDFs longos** | PDFs extensos podem ter trechos ignorados na busca inicial. | Quebrar as perguntas em escopos menores ou pedir citação direta do parágrafo/capítulo. |
| **Confusão entre conceitos genéricos e do texto** | A ferramenta às vezes complementava dados com seu conhecimento prévio. | Incluir a instrução restritiva: *"Responda apenas com dados explicitamente presentes nas fontes fornecidas"*. |

---

### 3. Valorização dessa Expertise pelo Mercado de Trabalho

O domínio de ferramentas como o **NotebookLM** aliados à **Engenharia de Prompts fundamentada em dados** é uma das habilidades mais valorizadas no ecossistema atual de tecnologia e corporativo:

* **SME de IA / Analista de RAG:** Profissionais que sabem curar dados e extrair respostas precisas de bases proprietárias evitam custos milionários de retreinamento de modelos.
* **Aumento drástico de produtividade:** A capacidade de transformar 500 páginas de relatórios/PDFs em resumos executivos acionáveis em minutos é um diferencial estratégico para cargos de liderança, produto e pesquisa.
* **Mitigação de riscos e Compliance:** Saber restringir a I.A para responder *apenas* com base em documentos oficiais reduz drasticamente riscos jurídicos e vazamento de alucinações operacionais.

---

## 📑 Resultado Final Consolidado

### 📊 1. Resumo Estruturado do Assunto

#### **A. O que é Engenharia de Prompts?**
A engenharia de prompts é a disciplina de estruturar textos de entrada para que modelos de linguagem (LLMs) gerem resultados mais precisos, alinhados e úteis. As melhores práticas incluem:
* Fornecer instruções claras e diretas.
* Incluir exemplos concretos (*Few-Shot*).
* Especificar o papel do sistema (*Persona*) e o formato de saída desejado (tabelas, listas, JSON).

#### **B. Retrieval-Augmented Generation (RAG) e Notebooks de IA**
Sistemas baseados em RAG combinam a capacidade de raciocínio das LLMs com bases de dados privadas. O NotebookLM atua exatamente como um ambiente RAG pronto para uso: ele lê as fontes enviadas, indexa o conteúdo e restringe o escopo de respostas ao contexto provido pelo usuário.

---

### 📖 2. Glossário de Conceitos Aprendidos

* **Prompt:** Instrução em linguagem natural enviada a um modelo de IA.
* **Contexto:** O conjunto de informações ou documentos fornecidos à IA para orientar sua resposta.
* **RAG (Retrieval-Augmented Generation):** Técnica que busca informações em uma base externa antes de gerar a resposta final via LLM.
* **Few-Shot Prompting:** Técnica de incluir um ou mais exemplos no prompt para orientar o formato e o estilo da resposta.
* **Chain-of-Thought (CoT):** Estratégia de instruir a IA a "pensar passo a passo" antes de chegar à resposta final, melhorando a precisão em problemas lógicos.
* **Alucinação:** Situação em que a IA gera informações falsas ou não comprovadas pelos dados de treinamento/fonte.

---

### 🔁 3. Guia de Prompts Reutilizáveis (Para Futuras Revisões)

Abaixo estão os templates de prompts validados e prontos para reutilização em qualquer caderno do NotebookLM:

#### **Prompt para Resumo Executivo**
```text
Atue como um sintetizador de conteúdo técnico. Com base no material carregado, crie um resumo executivo cobrindo:
1. O objetivo principal dos documentos.
2. Os 3 principais pontos ou descobertas.
3. Conclusões ou recomendações finais.
Mantenha o tom profissional e use listas em tópicos.
