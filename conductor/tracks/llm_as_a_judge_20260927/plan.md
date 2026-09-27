# Plano de Implementação: Adicionar fundamentação e discussão de LLM-as-a-Judge na monografia

## Visão Geral das Fases
O trabalho está estruturado em 4 fases sequenciais para garantir rigor bibliográfico, integração textual contínua e validação de compilação da monografia em LaTeX.

---

## Fase 1: Levantamento Bibliográfico e Curadoria de Artigos sobre LLM-as-a-Judge

- [x] Task: Pesquisa e Curadoria de Artigos Científicos sobre LLM-as-a-Judge 5e07eb8
    - [x] Pesquisar e selecionar artigos de referência (Zheng et al. 2023 - MT-Bench/Chatbot Arena; Kim et al. 2023 - Prometheus; Es et al. 2023 - RAGAS; Chen et al. 2024 - LLM-as-a-Judge survey).
    - [x] Mapear as contribuições de cada artigo: arquiteturas de avaliação, métricas (pairwise vs. pointwise), vieses conhecidos e mitigação.
    - [x] Estruturar fichamento sintético dos artigos com foco na aplicação a diálogos e personas em jogos.

- [x] Task: Atualização e Validação do Banco Bibliográfico (`referencias.bib`) 5e07eb8
    - [x] Formatar as entradas BibTeX completas para todos os artigos selecionados.
    - [x] Integrar as entradas no arquivo `monografia/referencias.bib`.
    - [x] Validar a integridade sintática do arquivo BibTeX.

- [x] Task: Conductor - User Manual Verification 'Fase 1: Levantamento Bibliográfico e Curadoria de Artigos sobre LLM-as-a-Judge' (Protocol in workflow.md) 348d900

---

## Fase 2: Fundamentação Teórica no Capítulo 2 (Referencial Teórico)

- [x] Task: Elaboração da Subseção Teórica de LLM-as-a-Judge em `cap2_referencial_teorico.tex` 1e9b2fe
    - [x] Analisar o fluxo atual do Capítulo 2 para posicionar harmonicamente a nova subseção.
    - [x] Redigir a subseção abordando conceitos fundamentais, comparação com métricas léxicas/n-gramas e modos de julgamento (pairwise vs pointwise).
    - [x] Abordar os vieses inerentes documentados na literatura (position bias, verbosity bias, self-enhancement bias) e estratégias de atenuação.
    - [x] Inserir chamadas de citação cruzada `\cite{...}` compatíveis com o banco BibTeX.

- [x] Task: Conductor - User Manual Verification 'Fase 2: Fundamentação Teórica no Capítulo 2 (Referencial Teórico)' (Protocol in workflow.md) 1e9b2fe

---

## Fase 3: Detalhamento Metodológico no Capítulo 4 (Metodologia)

- [x] Task: Formalização do Mecanismo de Avaliação no Capítulo 4 (`cap4_metodologia.tex`) e01d2a2
    - [x] Mapear onde a avaliação e métricas são descritas no Capítulo 4.
    - [x] Enriquecer a descrição metodológica explicitando o papel do LLM como juiz avaliador das respostas dos NPCs.
    - [x] Detalhar o pipeline de avaliação: formulação dos prompts de avaliação, rubricas de fidelidade à persona, preservação de segredos e integração com o framework RAGAS.

- [x] Task: Conductor - User Manual Verification 'Fase 3: Detalhamento Metodológico no Capítulo 4 (Metodologia)' (Protocol in workflow.md) e01d2a2

---

## Fase 4: Discussão Crítica no Capítulo 6 e Validação de Compilação

- [ ] Task: Atualização das Discussões e Limitações no Capítulo 6 (`cap6_resultados_discussoes.tex`)
    - [ ] Analisar as seções de resultados existentes para conectar os dados empíricos ao comportamento do juiz LLM.
    - [ ] Redigir parágrafos de discussão crítica sobre a concordância e limitações observadas no LLM-as-a-Judge durante os testes de estresse e diálogo investigativo.
    - [ ] Relacionar os achados experimentais com as discussões teóricas introduzidas no Capítulo 2.

- [ ] Task: Compilação Completa e Auditoria da Monografia
    - [ ] Executar pipeline de compilação da monografia (`pdflatex` + `bibtex` + `pdflatex` x2).
    - [ ] Verificar logs de compilação para garantir ausência de citações não resolvidas (`?`) ou warnings críticos.
    - [ ] Validar visualmente o PDF final gerado (`monografia/main.pdf`).

- [ ] Task: Conductor - User Manual Verification 'Fase 4: Discussão Crítica no Capítulo 6 e Validação de Compilação' (Protocol in workflow.md)
