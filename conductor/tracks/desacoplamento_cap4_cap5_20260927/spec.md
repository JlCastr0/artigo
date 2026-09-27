# Especificação do Track: Resolver Sobreposição entre Capítulo 4 e Capítulo 5

## 1. Visão Geral
Esta track tem por objetivo refatorar e desacoplar cirurgicamente o conteúdo entre o **Capítulo 4 (Metodologia)** e o **Capítulo 5 (Implementação)** na monografia de TCC. Atualmente, a Seção 4.4 do Capítulo 4 detalha excessivamente a engenharia de software da triagem ReAct, listando os comandos sintáticos de baixo nível (`[BUSCAR_CRONOGRAMA_MANHA]`, etc.) e o despacho de arquivos JSON, repetindo quase verbatim a discussão e a Tabela 5.1 do Capítulo 5. 

O escopo é estrito: delimitar o Capítulo 4 à formalização do modelo conceitual de particionamento e ciclo ReAct, mantendo a tabela de gramática técnica de comandos e os detalhes de despacho em código exclusivamente no Capítulo 5.

## 2. Objetivos
1. **Capítulo 4 (Metodologia - Seção 4.4):** Refatorar a Seção 4.4 para focar no princípio metodológico do *Agentic RAG* e na justificação científica da fragmentação temporal dinâmica (*Dynamic Chunking*), explicando a lógica de triagem conceitual sem antecipar comandos sintáticos e gramática de implementação.
2. **Capítulo 5 (Implementação - Seção 5.4):** Preservar como ponto focal único da engenharia de software a gramática de comandos ReAct, a tabela descritiva (`Tabela 5.1`), a expressão regular e a integração C#/Unity.
3. **Escopo Estrito:** Nenhuma outra seção, apêndice ou pendência (como TODOs em outras seções) será alterada nesta track.

## 3. Requisitos Estruturais
- **RE01:** No Capítulo 4 (`monografia/capitulos/cap4_metodologia.tex`), reformular a Seção 4.4 substituindo a enumeração de comandos sintáticos brutos (`[BUSCAR_...]`) por uma explicação conceitual do particionamento e roteamento ReAct.
- **RE02:** No Capítulo 5 (`monografia/capitulos/cap5_desenvolvimento_implementacao.tex`), garantir que a Seção 5.4 e a Tabela 5.1 continuem como a referência canônica completa da implementação da triagem, sem redundâncias externas.
- **RE03:** Garantir transição textual fluida e referências cruzadas adequadas (e.g., o Cap. 4 apontando que os detalhes de codificação e a gramática de comandos são apresentados na Seção \ref{sec:dev_triagem}).
- **RE04:** Manter a compilação limpa do LaTeX (`pdflatex`), com zero erros de compilação ou citações quebradas.

## 4. Fora de Escopo (Out of Scope)
- Resolução de `[TODO]` em outras seções (Fase 1, hardware, etc.).
- Alteração nos capítulos de resultados, referencial teórico ou introdução.
- Modificação dos apêndices ou arquivos de código Unity/C#.

## 5. Critérios de Aceitação
- [ ] Seção 4.4 reescrita com foco metodológico/conceitual puro, sem duplicar a gramática de comandos do Cap. 5.
- [ ] Referência cruzada elegante entre o Capítulo 4 e a Seção 5.4 do Capítulo 5.
- [ ] Tabela de comandos mantida exclusivamente no Capítulo 5.
- [ ] Compilação de `monografia/main.tex` validada com sucesso via `pdflatex`.
