---

### 2. `Readme.md`
Este arquivo é o guia de uso documentado, contendo a explicação de como o repositório funciona, instruções de produção e exemplos práticos para colocar no seu GitHub.

```markdown
# Arquivista Crítico (v5.1) — Skill de Resumos Estruturados para o Claude

Este repositório contém a especificação técnica e o prompt de produção para transformar o Claude (Anthropic) numa ferramenta de **Análise Crítica e Auditoria Factual de Livros em PDF**. 

Esta skill foi desenhada especificamente para gerar resumos de alta densidade informacional, blindados contra alucinações, focados na extração de frameworks práticos e mapeamento do perfil cognitivo/estilístico do autor. O resultado serve como uma **Base de Conhecimento Pessoal (Segunda Mente)** otimizada para futuras consultas da própria IA.

---

## 📖 Instruções Claras de Uso (Workflow de Produção)

### Passo 1: Preparação do Arquivo
Certifique-se de que o PDF do livro possui uma camada de texto legível (OCR). Evite arquivos digitalizados puramente como imagem antiga, pois isso quebra as travas de validação estrita da IA.

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

## 💡 Como Usar os Resumos Gerados para Futuras Consultas

A grande vantagem deste método é a **economia de tokens e a precisão do contexto**. Quando precisar resolver um problema complexo usando a filosofia daquele autor, você **não precisa enviar o livro de 400 páginas novamente**. 

Basta fazer o upload do resumo compacto de 2 páginas que a skill gerou e instruir o Claude.

### 🌟 Exemplo Prático de Prompt Futuro (Consulta Avançada)

> *"Claude, estou a estruturar a estratégia de liderança e comunicação da minha startup durante uma fase crítica de pivotagem de produto. Vou anexar aqui o **Resumo de Referência Futura** do livro 'Conversas Difíceis' que geramos anteriormente. Com base estritamente no perfil cognitivo do autor e nos frameworks de 'Distinção entre Intenção e Impacto' mapeados nas seções 2 e 3 deste resumo, forneça-me um roteiro prático passo a passo de como devo abordar o meu cofundador sem criar atritos desnecessários."*

Isso força a IA a simular perfeitamente a linha de pensamento do autor a partir de uma base confiável e auditada, sem risco de desvios conceituais ou alucinações históricas.
