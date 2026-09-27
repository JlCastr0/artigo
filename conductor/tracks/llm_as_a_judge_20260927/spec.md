# Especificação do Track: Adicionar fundamentação e discussão de LLM-as-a-Judge na monografia

## 1. Visão Geral
Este track tem por objetivo pesquisar, formalizar e incorporar o paradigma **LLM-as-a-Judge** (Modelos de Linguagem de Grande Escala como Avaliadores) na monografia de TCC. O projeto investiga a geração dinâmica de diálogos para NPCs em jogos de investigação. Como a avaliação manual humana em larga escala é custosa e métricas baseadas em n-gramas (BLEU, ROUGE) são insuficientes para avaliar coerência semântica e fidelidade à persona, o paradigma *LLM-as-a-Judge* (junto a frameworks como RAGAS) atua como o pilar avaliativo central da pesquisa.

## 2. Objetivos
1. **Levantamento Bibliográfico:** Identificar e fichar artigos científicos seminais e contemporâneos sobre o tema (e.g., Zheng et al. 2023 "Judging LLM-as-a-Judge", Kim et al. 2023 "Prometheus", Es et al. 2023 "RAGAS", Saha et al. 2024 "Branch-Solve-Merge", etc.).
2. **Atualização do Banco Bibliográfico (`referencias.bib`):** Incluir entradas BibTeX completas, padronizadas e verificadas para os artigos selecionados.
3. **Capítulo 2 (Referencial Teórico):** Redigir uma subseção dedicada explicando a mecânica de funcionamento do LLM-as-a-Judge, tipos de avaliação (pairwise ranking vs. direct point-wise scoring via rubricas), e os desafios conhecidos da literatura (vieses de posição, verbosidade, auto-favorecimento).
4. **Capítulo 4 (Metodologia):** Detalhar como o LLM-as-a-Judge foi parametrizado e operacionalizado no experimento do TCC (prompts de julgamento, métricas do RAGAS adaptadas, critérios de fidelidade à persona e contenção de segredo investigativo).
5. **Capítulo 6 (Resultados e Discussões):** Incluir discussão crítica analisando a confiabilidade do juiz sintético em relação aos diálogos gerados, análise de casos de divergência e limitações metodológicas encontradas.

## 3. Requisitos Funcionais e Estruturais
- **RF01:** Pesquisa e seleção de pelo menos 4 a 6 artigos de alto impacto sobre LLM-as-a-Judge e métricas de julgamento automatizado.
- **RF02:** Criação e integração das entradas BibTeX em `monografia/referencias.bib`.
- **RF03:** Inserção de subseção teórica no Capítulo 2 (`monografia/capitulos/cap2_referencial_teorico.tex`) com linguagem científica e citações no formato ABNT (`\cite{...}`).
- **RF04:** Adequação do Capítulo 4 (`monografia/capitulos/cap4_metodologia.tex`) para explicitar o protocolo de avaliação com o LLM-as-a-Judge.
- **RF05:** Atualização da seção de discussões no Capítulo 6 (`monografia/capitulos/cap6_resultados_discussoes.tex`) contextualizando os resultados à luz das evidências da literatura sobre acurácia e vieses do juiz LLM.
- **RF06:** Compilação do documento LaTeX (`pdflatex` + `bibtex`) sem erros ou referências quebradas (`?` ou warnings críticos).

## 4. Requisitos Não Funcionais
- **RNF01 (Padrão Acadêmico):** Respeitar as diretrizes de redação acadêmica (tom impessoal, precisão conceitual, conformidade ABNT/UEA).
- **RNF02 (Integridade Teórica):** Discutir transparentemente os vieses inerentes ao LLM-as-a-Judge (position bias, verbosity bias, egocentric bias) e como foram mitigados no trabalho.

## 5. Critérios de Aceitação
- [ ] Entradas BibTeX adicionadas e validadas sintaticamente em `referencias.bib`.
- [ ] Subseção de LLM-as-a-Judge inserida no Capítulo 2 com revisão de literatura aprofundada.
- [ ] Protocolo metodológico do juiz detalhado no Capítulo 4.
- [ ] Discussão de resultados no Capítulo 6 abordando o desempenho e os limites do juiz.
- [ ] Documento PDF da monografia compilando perfeitamente sem erros de compilação ou citações não resolvidas.
