# Tech Stack: Monografia de TCC e Artigos Científicos

## 1. Documentação e Tipografia
- **Linguagem Principal:** LaTeX2e
- **Motor de Compilação:** `pdflatex` com suporte a `bibtex`
- **Classes e Templates:**
  - `report` (com customizações ABNT/UEA para monografia)
  - `sbc-template.sty` e `sbc.bst` (Sociedade Brasileira de Computação para artigos)
  - `beamer` (para apresentação de slides de defesa)
- **Pacotes Principais:**
  - Tipografia e Estrutura: `times`, `geometry`, `setspace`, `titlesec`, `fancyhdr`, `babel`, `inputenc`, `fontenc`
  - Tabelas e Figuras: `graphicx`, `booktabs`, `tabularx`, `caption`, `subcaption`, `float`, `placeins`
  - Diagramação e Gráficos: `tikz` (com bibliotecas `shapes.geometric`, `arrows`, `positioning`, `calc`, `fit`, `backgrounds`), `pgfplots`
  - Citações e Hiperlinks: `cite`, `url`, `hyperref`
  - Listagens de Código: `listings`

## 2. Scripts e Automação
- **Linguagem:** Python 3
- **Utilidades:** Scripts de pós-processamento, conversão e validação textual (ex: `rease-submission/format_rease.py`)

## 3. Tecnologias de Pesquisa e Modelagem (Contexto Experimental)
- **Modelos de Linguagem (LLMs):** Modelos de ponta (ex: GPT-4o, Claude 3.5, LLaMA-3, Mistral) avaliados em geração textual e *persona adherence*.
- **Estruturação de Dados:** JSON (especificação semântica de perfis de personagens, memórias e segredos investigativos).
- **Métricas e Avaliação Automatizada:** Framework RAGAS (Faithfulness, Answer Relevance) e metodologia *LLM-as-a-Judge* (usando prompts de julgamento automatizados com critérios de consistência de persona e contenção de segredo).
