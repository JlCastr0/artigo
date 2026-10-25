# Especificação Técnica: Revisão Estilística e Polimento Acadêmico da Monografia

## Visão Geral
Esta track tem como objetivo realizar uma revisão estilística profunda em todo o texto da monografia em `monografia/`, elevando o registro de linguagem aos padrões rigorosos da norma culta acadêmica (ABNT / UEA / SBC). A intervenção removerá o estilo de "tópicos de apresentação", excesso de marcações em negrito (`\textbf`) no meio de parágrafos, listas fragmentadas e títulos coloquiais, substituindo-os por uma prosa científica contínua, elegante, analítica e estritamente impessoal.

## Requisitos Funcionais (Escopo da Revisão)
1. **Capítulo 6 (Resultados e Discussões):**
   - Reestruturar o texto sob a Tabela 6.4, eliminando negritos no meio de frases ao citar construtos psicométricos e valores numéricos.
   - Ajustar o título da Subseção 6.5.2 de `Dedução Investigativa e Resolução do Caso (100\% de Acerto)` para `Dedução Investigativa e Resolução do Caso Policial`, incorporando os 100% de acerto dentro da argumentação discursiva.
   - Transformar a lista de casos fenomenológicos (Subseção 6.5.4: Blefe de P1, Injeção de P4, Psicologia de P9, etc.) em texto discursivo fluido e coeso, eliminando cabeçalhos em negrito em itens enumerados.
   - Polir a discussão das Seções 6.2 e 6.3 referente aos quatro modelos de linguagem, garantindo transições suaves e terminologia sóbria.
2. **Capítulo 4 (Metodologia e Arquitetura):**
   - Converter a listagem dos Blocos 0 a 5 do questionário pós-teste (Subseção 4.6.4) em uma discussão metodológica integrada em prosa discursiva, evitando subtópicos repetitivos em negrito.
   - Revisar ocorrências de negrito e pontuações coloquiais nos demais trechos do capítulo.
3. **Capítulos 1, 2, 3, 5 e 7:**
   - Varredura geral para substituir negritos isolados no corpo de sentenças por itálico ou tipografia padrão.
   - Garantir a uniformidade da voz passiva sintética e da terceira pessoa impessoal ("constatou-se", "observa-se", "mensurou-se").

## Requisitos Não-Funcionais e Critérios de Aceitação
- **Contagem Estrita de Páginas:** A monografia deve ser mantida exatamente no intervalo de **74 a 75 páginas totais** no `main.pdf`.
- **Integridade dos Dados:** Nenhuma alteração de valores numéricos, métricas do RAGAS, notas do GEQ, escore do SUS ou conclusões do estudo com os 10 participantes do TCLE.
- **Compilação Perfeita:** Compilação limpa via `bibtex` e `pdflatex` com zero erros.
- **Registro Formal:** Texto estritamente científico e acadêmico, sem jargões de relatório executivo ou linguagem promocional.

## Fora de Escopo
- Alteração da estrutura de tabelas consolidadas ou de referências bibliográficas.
- Modificação dos apêndices (perguntas ou formulários canônicos).
