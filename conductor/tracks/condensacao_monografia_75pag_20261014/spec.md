# Especificação Técnica: Condensação e Otimização da Monografia (Meta: 75 Páginas)

## Visão Geral
Esta track tem como objetivo reestruturar e condensar cirurgicamente a monografia localizada em `monografia/`, reduzindo a extensão atual de 88 páginas para uma meta estrita de **74 a 76 páginas** (alvo: 75 páginas completas), atendendo às expectativas de concisão e maturidade acadêmica da banca examinadora da UEA. A otimização será conduzida sem qualquer perda de rigor científico, mantendo integralmente todas as formulações matemáticas, dados experimentais, as 50 perguntas adversárias de estresse e a discussão dos 10 participantes do estudo piloto com TCLE.

## Requisitos Funcionais (Escopo de Redução)
1. **Capítulos 1 e 2 (Desduplicação Econômica e Teórica):**
   - Eliminar a duplicação do cálculo de custo de tokens (50.000 cópias x bilhões de tokens) entre as Seções 1.2.1 e 2.2.1.
   - Manter a contextualização concisa no Capítulo 1 e a formalização matemática completa no Capítulo 2.
   - Enxugar a Seção 2.5.1 referente a vieses do LLM-as-a-Judge (-2 a -3 páginas).
2. **Capítulo 4 (Metodologia e Narrativa Investigativa):**
   - Unificar a narrativa prolixa da Crônica das Horas (Seção 4.2.2) com a análise de Momentos-Chave da Investigação (Seção 4.3.2) através de uma tabela cronológico-investigativa integrada.
   - Aplicar compactação de listas (`noitemsep`, `topsep=2pt`) e diminuir espaçamentos excessivos (-4 a -5 páginas).
3. **Capítulo 6 (Resultados e Discussões):**
   - Sintetizar as transcrições das respostas dos quatro modelos avaliados nas Tabelas 6.2 a 6.5 (Categorias 1 a 5), substituindo blocos de texto redundantes por excertos essenciais (*snippets* de 2 a 3 linhas com reticências).
   - Preservar integralmente as tabelas quantitativas de RAGAS, o perfil demográfico dos 10 voluntários (P1 a P10) e a análise qualitativa profunda dos 5 casos marcantes (-3 a -4 páginas).
4. **Apêndices C e D (Tipografia e Compactação de Instrumentos):**
   - Reestruturar a bateria de 50 testes do Apêndice C em formato de duas colunas ou tabela compacta.
   - Diagramar o questionário pós-teste do Apêndice D de forma densa e profissional com espaçamento simples, reduzindo réguas horizontais redundantes (-2 páginas).

## Requisitos Não-Funcionais e Critérios de Aceitação
- **Total de Páginas:** O documento final `main.pdf` deve conter exatamente entre **74 e 76 páginas** (alvo: 75 páginas).
- **Integridade Científica:** Zero remoções de tabelas de métricas, referências bibliográficas, formulações matemáticas ou achados empíricos.
- **Compilação Limpa:** O documento deve compilar perfeitamente via `bibtex` e `pdflatex` com zero erros e warnings tratados.
- **Conformidade Normativa:** Manter a estrita conformidade com as diretrizes ABNT e normas da Universidade do Estado do Amazonas (EST/UEA).

## Fora de Escopo
- Remoção de qualquer uma das 50 perguntas da bateria de estresse dialógico.
- Alteração ou exclusão de qualquer participante dos 10 perfis simulados da EST/UEA.
- Supressão de capítulos ou de fundamentações teóricas canônicas (GEQ, SUS, PENS, CASA, RAGAS).
