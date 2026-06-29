# 📚 Arquivista Crítico (v5.1) — Engenharia de Resumos Estruturados via Claude Projects

> **Sugestões de Títulos para o seu Repositório:**
> * `claude-project-arquivista-critico`
> * `knowledge-archivist-project`
> * `prompt-rag-resumo-critico`

## 🎯 Descrição do Projeto

O **Arquivista Crítico** é uma especificação técnica de engenharia de prompt desenhada para transformar a área de **Projetos (Projects)** do Claude (Anthropic) numa central automatizada de **Análise Crítica e Auditoria Factual de Livros em PDF**.

Ao configurar esta Skill nas diretrizes estruturais do seu Claude Project, você elimina a necessidade de copiar e colar prompts manuais a cada conversa. Toda vez que iniciar um chat novo e anexar um livro dentro desse projeto, o Claude aplicará automaticamente um processo interno de auditoria (`<thinking>`) com ancoragem factual extrema. O sistema varre o arquivo anexado para mapear de forma cirúrgica o perfil cognitivo do autor (idiossincrasias, tom, vieses) e extrair os frameworks práticos mais importantes. O resultado é um arquivo condensado em Markdown (`.md`), blindado contra alucinações e otimizado para servir como uma **Base de Conhecimento Pessoal (Segunda Mente)** para consultas futuras de humanos ou de outras instâncias de IA, economizando milhares de tokens.

---

## 🧠 Benefícios Técnicos e Arquitetura Cognitiva

Ao utilizar o **Arquivista Crítico**, você cria um pipeline de dados otimizado para Large Language Models (LLMs):
* **Automação via Infraestrutura (No-Paste):** O prompt mestre fica fixado na memória raiz do projeto do Claude. Você só precisa arrastar e soltar o livro.
* **Eficiência de Contexto (Token Saving):** Reduz um livro inteiro de ~400 páginas para uma estrutura densa de 2 a 3 páginas. Isso diminui o consumo de tokens em mais de 95% nas consultas subsequentes.
* **Sandbox Baseado em Fatos:** Evita que o Claude misture o conteúdo do livro com alucinações geradas pelo senso comum da internet, restringindo a IA estritamente à lógica do autor.
* **Rastreabilidade:** As exigências de citação de capítulos ou seções funcionam como um mecanismo ágil de checagem interna para auditoria humana rápida.

---

## 📖 Instruções de Configuração e Uso (Workflow de Produção)

### Passo 1: Criar o Projeto no Claude
1. Acesse o Claude.ai (necessário plano Pro ou Team).
2. No menu lateral ou na página inicial, clique em **Projects** e selecione **Create Project**.
3. Escolha um nome para o seu projeto (ex: *Arquivista Crítico de Livros*).

### Passo 2: Definir as Instruções Coletivas (Instanciação da Skill)
1. Dentro do seu novo projeto, clique em **Set Custom Instructions** (Definir Instruções Personalizadas) no painel direito.
2. Copie e cole todo o conteúdo do arquivo `instrucoes.md` deste repositório dentro da caixa de texto de instruções.
3. Clique em **Save**. Pronto! A inteligência de auditoria agora está congelada na raiz de todos os chats que você abrir aqui dentro.

### Passo 3: Geração Automatizada do Resumo
1. Com o projeto configurado, abra um novo chat **dentro dele**.
2. Faça o upload do arquivo PDF do livro (certifique-se de que o PDF possui camada de texto legível por OCR).
3. Escreva apenas uma mensagem simples de ativação, por exemplo: *"Gere o Resumo de Referência Futura deste livro."*
4. O Claude processará a tag `<thinking>` em segundo plano e entregará a saída oficial rigorosamente estruturada.

### Passo 4: Armazenamento Estruturado (Segunda Mente)
Copie a saída gerada e salve localmente num arquivo de texto usando a extensão `.md` (Markdown). Adote o seguinte padrão de nome de arquivo para organização:
`sobrenome-autor_titulo-do-livro.md` (Exemplo: `kahneman_rapido-e-devagar.md`).

---

## 🚀 Exemplos Práticos de Uso para Consultas Avançadas

Depois de mapear seus livros técnicos, doutrinas ou manuais e alimentar o seu ecossistema, você poderá cruzar os dados ou aplicar os resumos gerados em cenários do seu dia a dia profissional. Veja estes três exemplos de prompts avançados para usar no Claude:

### 🌟 Exemplo 1: Psicologia e Saúde Mental (Formulações Clínicas e Abordagens)
> **Contexto:** Você gerou o resumo crítico de um manual clássico sobre Terapia Cognitivo-Comportamental (TCC) ou um tratado de psicopatologia de referência.
>
> **Prompt para o Claude:**
> *"Claude, estou estruturando a formulação de caso de um paciente fictício que apresenta sintomas acentuados de ansiedade generalizada e padrões repetitivos de catastrofização. Estou anexando o **Resumo de Referência Futura** do livro de TCC que consolidamos no projeto. Com base estritamente nos frameworks de 'Identificação de Pensamentos Automáticos' e 'Questionamento Socrático' mapeados na Seção 3 e herdando as lentes metodológicas do autor detalhadas na Seção 2, crie uma estratégia de intervenção contendo 3 perguntas reflexivas para a próxima sessão. Não utilize abordagens fora do escopo deste resumo."*

### 🌟 Exemplo 2: Advocacia e Direito (Análise de Casos com base em Livros de Leis/Doutrinas)
> **Contexto:** Você gerou o resumo crítico de um livro de doutrina jurídica robusta ou comentários estruturados a códigos legais.
>
> **Prompt para o Claude:**
> *"Claude, estou analisando um caso complexo de quebra de contrato comercial devido a um evento de força maior imprevisto. Anexei aqui o **Resumo de Referência Futura** do livro de Doutrina de Direito Civil sobre Responsabilidade Contratual que mapeamos anteriormente. Utilizando exclusivamente a interpretação do autor sobre o nexo de causalidade e as excludentes de responsabilidade civil documentadas na Seção 3, faça um parecer preliminar apontando os pontos fortes e os pontos fracos do argumento da nossa defesa. Cite os termos originais e jargões do autor mapeados na Seção 4 (Glossário)."*

### 🌟 Exemplo 3: Engenharia de Produto, Inovação e Growth (Cenário Técnico)
> **Contexto:** Você gerou o resumo crítico do livro *"O Dilema da Inovação"* de Clayton Christensen.
>
> **Prompt para o Claude:**
> *"Claude, atuamos no mercado de SaaS para logística e um concorrente menor começou a oferecer uma ferramenta gratuita, simplificada, mas muito veloz, ameaçando nossa base de clientes de entrada. Anexei aqui o **Resumo de Referência Futura** do livro 'O Dilema da Inovação' (Clayton Christensen). Utilizando exclusivamente o conceito de 'Inovação Disruptiva vs. Sustentável' e as limitações de mercado documentadas nas seções 3 e 5 deste resumo, faça um diagnóstico do nosso cenário estratégico e sugira duas linhas de defesa que a nossa engenharia de produto pode adotar."*
