# Diretrizes do Projeto de Monografia e Artigo Científico

Este documento estabelece as convenções estruturais, estilísticas e tipográficas obrigatórias para os textos acadêmicos deste repositório (monografia, artigos e apresentações).

## 1. Regras Tipográficas e de Estilo em LaTeX

- **Sem Negrito dentro de Parágrafos (REGRA CRÍTICA):**
  - **NUNCA** utilize negrito (`\textbf{}`) no meio, no início ou no corpo de parágrafos de texto corrido como forma de ênfase ou pseudo-tópico.
  - O uso de `\textbf{}` é restrito a títulos de itens formais em listas (`\begin{itemize}` ou `\begin{enumerate}`) quando explicitamente exigido pela estrutura, ou em cabeçalhos de tabelas e comandos de estruturação do documento.
  - Para ênfases terminológicas indispensáveis ou termos em língua estrangeira, utilize itálico (`\textit{}`), mantendo a sobriedade da prosa acadêmica.

- **Evitar Travessões (`---`):**
  - **NUNCA** utilize travessões longos (`---` ou `—`) para orações intercaladas ou incisos explicativos. Se encontrar travessões em qualquer momento no texto, reescreva-os obrigatoriamente, substituindo-os por vírgulas, parênteses sóbrios ou reestruturação frasal.

- **Sem Parênteses em Tópicos e Bullet Points:**
  - **NÃO** utilize parênteses dentro de listas com marcadores (`\begin{itemize}` ou `\begin{enumerate}`), seja nos rótulos e títulos dos itens (como traduções ou siglas) ou no corpo das descrições.
  - Termos em língua estrangeira, siglas e especificações devem ser integrados à oração de forma discursiva e fluida, utilizando vírgulas ou conectivos adequados, evitando incisos parentéticos.
  - **Listas Curtas em Prosa (REGRA CRÍTICA):** Sempre que houver uma série de itens ou *bullet points* de até 3 elementos, é FORTEMENTE RECOMENDADO incorporá-los diretamente como prosa contínua (parágrafos), preservando a cadência da redação acadêmica e evitando fragmentações tópicas desnecessárias.

- **Fluidez Textual e Variação Estrutural (REGRA CRÍTICA CONTRA FÓRMULAS MECÂNICAS):**
  - **NUNCA** utilize fórmulas ordinais mecânicas ou sequenciamento burocrático de parágrafos que apenas disfarcem uma lista enumerada em texto corrido (como "Em primeiro lugar...", "Em segundo lugar...", "Como segunda diretriz...", "Por fim...", "Finalmente...").
  - As transições entre parágrafos devem ser estritamente temáticas, conceituais e discursivas, amarrando a ideia do parágrafo anterior com o próximo por meio da progressão lógica dos argumentos, contrastes teóricos ou implicações práticas, e não por marcadores de contagem.
  - Evite padrões frasais repetitivos ou fórmulas sintáticas mecânicas (por exemplo, listas de capítulos onde todos começam identicamente com "O Capítulo X analisa...", ou parágrafos sucessivos com abertura idêntica).
  - Varie a estrutura sintática das frases (alternando orações diretas, orações subordinadas e orações tópicas expressivas), garantindo ritmo elegante e naturalidade à prosa acadêmica.

- **Clareza, Sobriedade e Acessibilidade (REGRA CRÍTICA CONTRA VOCABULÁRIO REBUSCADO):**
  - Embora a formalidade e o rigor acadêmico sejam fundamentais e valorizados, o uso de palavras desnecessariamente difíceis, arcaicas ou pedantes complica a vida do leitor sem agregar valor científico.
  - Priorize a clareza, a concisão e a fluidez direta da explicação. Explique conceitos técnicos complexos de modo simples, preciso e natural, evitando maneirismos retóricos, vocabulário empolado ou afetações estilísticas que obscureçam as ideias centrais.

- **Foco Funcional na Descrição de UI (SEM Preciosismo de Código):**
  - **NÃO** descreva a interface de usuário detalhando nomes de componentes internos de engine ou minúcias de implementação (como \textit{Scroll View}, \textit{TextMeshPro}, \textit{TMP\_InputField}, nomes de \textit{prefabs} ou estruturas de nós), exceto se for indispensável no código de um script C\#.
  - Ao descrever telas e elementos visuais no texto, concentre-se na **função prática para o jogador**, na experiência de uso e no design da cena (como campo para digitação de perguntas livres, histórico cronológico da conversa e enquadramento visual dos personagens), mantendo o relato fluído, objetivo e focado na interação.

- **Concisão e Limite Estrito de Páginas (75 Páginas como Teto Máximo - REGRA CRÍTICA):**
  - **75 páginas NÃO é uma meta de preenchimento:** é um **LIMITE MÁXIMO ABSOLUTO** estabelecido para a banca examinadora.
  - **Quanto menor e mais conciso, melhor:** a prioridade é a densidade científica e a objetividade. Nunca infle parágrafos para atingir páginas.
  - **Eliminação ativa de redundâncias:** corte repetições conceituais entre capítulos (como reexplicar o mesmo problema ou método em múltiplos lugares), frases duplicadas e prolixidades. A diminuição da contagem total de páginas através de síntese rigorosa é ativamente incentivada.

## 2. Diretrizes Metodológicas e Fatos Canônicos dos Experimentos

- **Distinção Estrita entre os Experimentos (REGRA CRÍTICA):**
  - **Experimento com Jogadores Humanos (Validação Ecológica na Unity):** Os voluntários jogam o **jogo de verdade no motor gráfico Unity**, interagindo e dialogando livremente com **todo o elenco de suspeitos** da mansão Castelo (Alberto Castelo, Catarina Castelo, James e Silas Drummond). O jogador alterna entre os personagens na galeria policial, cruza depoimentos e deduz o verdadeiro culpado. **NUNCA** descreva o teste com humanos como restrito apenas a Alberto Castelo.
  - **Auditoria Computacional Automatizada (LLM-as-a-Judge com RAGAS):** Foi o **ÚNICO experimento em que exclusivamente Alberto Castelo foi avaliado**. A bateria de cinquenta perguntas de estresse dialógico foi submetida unicamente à persona de Alberto Castelo nos quatro modelos avaliados (Gemma-2, Qwen-2.5, Llama-3.1 e DeepSeek-R1), com o objetivo metodológico de isolar variáveis, controlar a verdade factual de referência (*ground-truth*) e padronizar o comparativo algorítmico entre as arquiteturas de LLM.

## 3. Estrutura do Repositório

- `monografia/`: Fonte LaTeX da monografia principal do TCC (dividida em `capitulos/` e `apendices/`).
- `rease-submission/`: Artigo formatado para submissão a periódico/conferência.
- `slides/`: Apresentação de defesa em Beamer.
- `conductor/`: Especificações e rastreamento de tarefas do projeto.
