# Inteligência Comportamental, Simulação de Futuros e RAG Factual para Decisões Financeiras

Um notebook de ciência de dados ponta a ponta e análises fundamentadas em RAG (Retrieval-Augmented Generation) projetado para avaliar padrões sazonais de dívidas, segmentar coortes de transações de usuários, calcular margens seguras de redução de orçamento e entregar planos de recuperação financeira personalizados alinhados às diretrizes de educação financeira do Banco Central.

---

## Visão Geral do Projeto

Despesas sazonais não planejadas e juros compostos frequentemente geram déficits no orçamento familiar. Este repositório fornece um fluxo de trabalho analítico e uma estrutura de Inteligência Generativa projetados para restaurar a estabilidade financeira por meio da otimização quantitativa do orçamento e interações de consultoria fundamentadas.

### Principais Objetivos

* **Segmentação de Coortes:** Identificar padrões de transação e a vulnerabilidade do usuário a picos sazonais de dívidas.
* **Cálculo de Margem Segura de Orçamento:** Computar limites de redução de gastos não essenciais sem impactar as despesas básicas de sobrevivência.
* **Orientação Baseada em RAG:** Utilizar Geração Aumentada por Recuperação (RAG) sobre frameworks oficiais de educação financeira para gerar planos de ação de recuperação compatíveis e personalizados.

---

## Stack Tecnológica

* **Linguagem:** Python 3.10+
* **Análise de Dados e Modelagem:** `pandas`, `NumPy`, `scikit-learn`
* **Visualização de Dados:** `matplotlib`, `seaborn`
* **IA Generativa & RAG:** `LangChain`, Vector Embeddings (FAISS / ChromaDB), Hugging Face / OpenAI APIs
* **Ambiente:** Jupyter Notebook / Google Colab

---

## Estrutura do Repositório

```text
├── data/
│   ├── raw_transactions.csv        # Histórico de transações de usuários anonimizado
│   └── central_bank_guidelines/    # Documentação de referência para o aterramento RAG
├── notebooks/
│   └── financial_health_analysis.ipynb  # Notebook principal de análises e modelagem
├── src/
│   ├── cohort_analysis.py          # Perfil de clientes e métricas de transação
│   ├── margin_calculator.py        # Algoritmos de redução segura de orçamento
│   └── rag_pipeline.py             # Configuração da cadeia RAG, embeddings e travas de segurança
├── requirements.txt
└── README.md

```

---

## Metodologia

1. **Análise Exploratória de Dados e Perfil de Coorte**
* Agrega despesas recorrentes fixas versus discricionárias entre as coortes de usuários.
* Isola anomalias sazonais de dívida (ex.: despesas de fim de ano, impostos anuais, mensalidades).


2. **Modelagem Quantitativa de Recuperação de Dívidas**
* Computa métricas de endividamento (DTI) e flexibilidade de renda disponível.
* Calcula dinamicamente margens de redução segura em categorias de gastos não essenciais.


3. **Base de Conhecimento RAG & Orientações Protegidas (Guardrails)**
* Incorpora frameworks regulatórios de educação financeira para orientação verificada.
* Aplica prompts de sistema para garantir recomendações financeiras transparentes e não predatórias.



---

## Guia de Início Rápido (Quick Start)

### 1. Pré-requisitos

Certifique-se de que o Python 3.10 ou superior está instalado em seu sistema.

### 2. Instalação

Clone este repositório e instale as dependências:

```bash
git clone https://github.com/your-username/financial-health-analytics.git
cd financial-health-analytics
pip install -r requirements.txt

```

### 3. Configuração do Ambiente

Crie um arquivo `.env` no diretório raiz e adicione suas chaves de API caso esteja executando o pipeline RAG:

```env
OPENAI_API_KEY=your_openai_api_key_here

```

### 4. Executando o Notebook

Inicie o Jupyter Lab e abra o notebook principal de análise:

```bash
jupyter lab notebooks/financial_health_analysis.ipynb

```

---
