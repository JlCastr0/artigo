# Plano de Implementação: Resolver Sobreposição entre Capítulo 4 e Capítulo 5

## Fase 1: Refatoração Metodológica da Seção 4.4 no Capítulo 4

- [x] Task: Reestruturação Textual e Conceitual da Seção 4.4 (`cap4_metodologia.tex`) c35c754
    - [x] Eliminar a enumeração de comandos sintáticos brutos de baixo nível (`[BUSCAR_...]`) da Seção 4.4.
    - [x] Redigir a explicação conceitual do ciclo ReAct e da hipótese da fragmentação temporal dinâmica (*Dynamic Chunking*).
    - [x] Inserir referência cruzada formal apontando para a Seção 5.4 (`\ref{sec:dev_triagem}`) do Capítulo 5 para a gramática de execução e despacho.

- [x] Task: Conductor - User Manual Verification 'Fase 1: Refatoração Metodológica da Seção 4.4 no Capítulo 4' (Protocol in workflow.md) c35c754

---

## Fase 2: Harmonização no Capítulo 5 e Validação de Compilação

- [x] Task: Revisão da Seção 5.4 no Capítulo 5 (`cap5_desenvolvimento_implementacao.tex`) ae717e4
    - [x] Verificar e assegurar que a Seção 5.4 e a Tabela 5.1 contêm a gramática completa e autossuficiente da engenharia ReAct.
    - [x] Ajustar a abertura da Seção 5.4 para referenciar formalmente a decisão metodológica estabelecida na Seção 4.4.

- [x] Task: Auditoria de Compilação LaTeX ae717e4
    - [x] Compilar a monografia com `pdflatex` + `bibtex` + `pdflatex`.
    - [x] Confirmar ausência de referências quebradas e validar fluidez de leitura.

- [x] Task: Conductor - User Manual Verification 'Fase 2: Harmonização no Capítulo 5 e Validação de Compilação' (Protocol in workflow.md) ae717e4
