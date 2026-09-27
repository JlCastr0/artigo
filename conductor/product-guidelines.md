# Product Guidelines: Monografia e Produções Científicas

## 1. Diretrizes de Redação Acadêmica (Estilo e Prosa)
- **Tom e Registro:** Impessoal, formal, objetivo e rigorosamente científico (voz passiva ou terceira pessoa, ex: "observa-se", "propõe-se", "foi avaliado").
- **Clareza e Precisão Conceitual:** Definir formalmente termos técnicos (LLMs, RAG, RAGAS, LLM-as-a-Judge, Prompt Injection, Hallucination, Personas) na primeira aparição antes de usar siglas ou jargões.
- **Estrutura Argumentativa:** Cada parágrafo deve conter uma ideia central bem delimitada, com fundamentação bibliográfica e encadeamento lógico entre seções e capítulos.
- **Língua:** Português formal para a monografia (norma culta, padrão UEA/ABNT), com resumos e artigos derivados também disponíveis em inglês acadêmico quando aplicável.

## 2. Padrões de Citação e Referências
- **Normas Bibliográficas:** Conformidade com ABNT NBR 6023 e diretrizes da UEA para a monografia, e formato SBC para artigos.
- **Rigor de Citação:** Toda afirmação factual, dado empírico ou modelo teórico deve referenciar a literatura primária (artigos de periódicos, conferências de primeira linha como ACL, EMNLP, NeurIPS, CHI, IEEE CoG, SBGames).
- **Consistência no BibTeX:** Chaves de citação semânticas e uniformes (ex: `autorAno`), com campos completos (`author`, `title`, `booktitle`/`journal`, `year`, `publisher`, `doi`).

## 3. Diretrizes de Apresentação Visual e Tipografia
- **Tipografia e Espaçamento:** Times New Roman, corpo 12, espaçamento 1.5 entre linhas, margens ABNT (superior 3cm, esquerda 3cm, inferior 2cm, direita 2cm).
- **Figuras e Gráficos:** Priorizar gráficos vetoriais e diagramas gerados nativamente em LaTeX (`TikZ`, `pgfplots`) ou imagens de alta resolução (mínimo 300 DPI) com legendas autoexplicativas e chamadas obrigatórias no texto.
- **Tabelas e Quadros:** Formatação limpa usando `booktabs` (linhas horizontais sem linhas verticais redundantes), alinhamento numérico consistente e fontes citadas logo abaixo.

## 4. Reprodutibilidade e Integridade Científica
- **Transparência Experimental:** Descrição completa de hiperparâmetros (temperatura, top_p), versões exatas de modelos de linguagem, bibliotecas (RAGAS, LangChain, LlamaIndex), prompts utilizados (incluídos nos apêndices) e sementes de aleatoriedade quando aplicável.
- **Ética e Limitações:** Discussão honesta sobre limitações metodológicas, custos de inferência, latência, viés de avaliação de LLMs (*LLM-as-a-Judge bias*) e aspectos éticos do uso de IA generativa em jogos.
