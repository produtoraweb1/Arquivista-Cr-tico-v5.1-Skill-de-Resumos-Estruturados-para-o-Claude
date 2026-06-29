# 📚 Arquivista Crítico (v5.1) — Engenharia de Resumos Estruturados para o Claude

> **Sugestões de Títulos para o seu Repositório:**
> * `claude-arquivista-critico`
> * `knowledge-archivist-skill`
> * `prompt-rag-resumo-critico`

## 🎯 Descrição do Projeto

O **Arquivista Crítico** é uma especificação técnica de engenharia de prompt (Skill) desenhada para transformar o Claude (Anthropic) numa ferramenta avançada de **Análise Crítica e Auditoria Factual de Livros em PDF**. 

Diferente de resumos passivos convencionais, esta skill força a IA a rodar um processo interno de auditoria (`<thinking>`) com ancoragem factual extrema. O sistema varre o arquivo anexado para mapear de forma cirúrgica o perfil cognitivo do autor (idiossincrasias, tom, vieses) e extrair os frameworks práticos mais importantes. O resultado é um arquivo condensado em Markdown (`.md`), blindado contra alucinações e otimizado estruturalmente para servir como uma **Base de Conhecimento Pessoal (Segunda Mente)** para consultas futuras de humanos ou de outras instâncias de IA, economizando milhares de tokens.

---

## 🧠 Benefícios Técnicos e Arquitetura Cognitiva

Ao utilizar o **Arquivista Crítico**, você cria um pipeline de dados otimizado para Large Language Models (LLMs):
* **Eficiência de Contexto (Token Saving):** Reduz um livro inteiro de ~400 páginas para uma estrutura densa de 2 a 3 páginas. Isso diminui o consumo de tokens em mais de 95% nas consultas subsequentes.
* **Sandbox Baseado em Fatos:** Evita que o Claude misture o conteúdo do livro com alucinações geradas pelo senso comum da internet, restringindo a IA estritamente à lógica do autor.
* **Rastreabilidade:** As exigências de citação de capítulos ou seções funcionam como um mecanismo ágil de checagem interna para auditoria humana rápida.

---

## 📖 Instruções Claras de Uso (Workflow de Produção)

### Passo 1: Preparação do Arquivo
Certifique-se de que o PDF do livro possui uma camada de texto legível (OCR). Evite arquivos digitalizados puramente como imagem antiga, pois isso quebra las travas de validação estrita da IA.

### Passo 2: Geração do Resumo Crítico
1. Abra um novo chat no **Claude (recomenda-se o modelo Claude 3.5 Sonnet ou superior)**.
2. Faça o upload do arquivo PDF do livro.
3. Copie o conteúdo completo do prompt presente no arquivo `instrucoes.md`.
4. Cole o prompt na mesma mensagem do arquivo anexo e envie.
5. Aguarde a IA processar a tag `<thinking>` (Raciocínio interno de auditoria) e estruturar a saída oficial.

### Passo 3: Armazenamento Estruturado (Segunda Mente)
Copie a saída gerada pela IA e salve localmente num arquivo de texto usando a extensão `.md` (Markdown). Adote o seguinte padrão de nome de arquivo para organização:
`sobrenome-autor_titulo-do-livro.md` (Exemplo: `kahneman_rapido-e-devagar.md`).
Guarde este arquivo no seu repositório local, Notion, Obsidian ou na sua pasta de conhecimento.

---

## 🚀 Exemplos Práticos de Uso para Consultas Avançadas

Depois de mapear seus livros usando a skill, você pode cruzar os dados ou aplicar os resumos gerados em cenários do seu dia a dia. Veja três exemplos de prompts avançados para usar no Claude:

### 🌟 Exemplo 1: Alinhamento de Expectativas e Conflitos (Liderança)
> **Contexto:** Você gerou o resumo crítico do livro *"Conversas Difíceis"*.
>
> **Prompt para o Claude:**
> *"Claude, estou a estruturar a estratégia de liderança e comunicação da minha startup durante uma fase crítica de pivotagem de produto. Vou anexar aqui o **Resumo de Referência Futura** do livro 'Conversas Difíceis' que geramos anteriormente. Com base estritamente no perfil cognitivo do autor e nos frameworks de 'Distinção entre Intenção e Impacto' mapeados nas seções 2 e 3 deste resumo, forneça-me um roteiro prático passo a passo de como devo abordar o meu cofundador sem criar atritos desnecessários."*

### 🌟 Exemplo 2: Tomada de Decisão e Estruturação de Processos (Cenário Corporativo)
> **Contexto:** Você gerou o resumo crítico do livro *"Princípios"* do Ray Dalio.
>
> **Prompt para o Claude:**
> *"Claude, estou reestruturando a dinâmica de rituais e reuniões semanais da minha equipe de operações para mitigar erros de comunicação ocultos. Estou anexando o **Resumo de Referência Futura** do livro 'Princípios' (Ray Dalio) que consolidamos. Com base estritamente no padrão de argumentação do autor e nos frameworks de 'Verdade Radical e Transparência Radical' mapeados na Seção 3, crie um guia prático de 4 regras de conduta para as nossas reuniões. Certifique-se de herdar o tom dogmático e analítico do autor descrito na Seção 2."*

### 🌟 Exemplo 3: Engenharia de Produto, Inovação e Growth (Cenário Técnico)
> **Contexto:** Você gerou o resumo crítico do livro *"O Dilema da Inovação"* de Clayton Christensen.
>
> **Prompt para o Claude:**
> *"Claude, atuamos no mercado de SaaS para logística e um concorrente menor começou a oferecer uma ferramenta gratuita, simplificada, mas muito veloz, ameaçando nossa base de clientes de entrada. Anexei aqui o **Resumo de Referência Futura** do livro 'O Dilema da Inovação' (Clayton Christensen). Utilizando exclusivamente o conceito de 'Inovação Disruptiva vs. Sustentável' e as limitations de mercado documentadas nas seções 3 e 5 deste resumo, faça um diagnóstico do nosso cenário estratégico e sugira duas linhas de defesa que a nossa engenharia de produto pode adotar."*
> 
