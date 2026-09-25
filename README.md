<div align="right"><a href="README.en.md">English version →</a></div>

# Rodrigo Martins

**Software Engineer | AI Engineering | Full Stack | RAG & Automation**

Desenvolvo sistemas corporativos que integram ERP, plataformas de BPM, APIs bancárias, mensageria e modelos de linguagem — e que ficam em produção, com gente usando todo dia.

Meu trabalho cobre o ciclo inteiro:

`processo de negócio → requisito → arquitetura → backend/frontend → API → banco → integração → testes → troubleshooting → operação e evolução`

Levantar a regra com quem é dono do processo costuma ser a parte mais difícil — e é ali que o sistema se decide, não no código.

---

## FlowMind AI

### RAG Engineering & Intelligent Automation Workbench

**→ [github.com/1Rodrigo97/flowmind-ai](https://github.com/1Rodrigo97/flowmind-ai)**

Bancada de trabalho para RAG: ingestão de documentos, recuperação vetorial, resposta ancorada na fonte e um laboratório para **medir** se a recuperação está de fato funcionando — em vez de confiar na impressão de que está.

**Implementado**

- Ingestão de **PDF, DOCX, MD e TXT**, com deduplicação por **SHA-256** e *chunking*
- **Embeddings** locais (`nomic-embed-text`, 768-d) e **busca vetorial** em **pgvector**
- **Grounded generation** com citação de fontes e **recusa explícita quando falta contexto** — o sistema diz que não sabe em vez de inventar
- **RAG Explorer** — inspeção do *retrieval*: os top-k trechos recuperados e seus scores
- **RAG Evaluation Lab** — experimentos reproduzíveis medindo **Hit@K, MRR, Precision@K e Recall@K**, comparando *baseline* × experimento
- **Reranking lexical BM25** — atrás de *feature flag*, desligado por padrão
- Perfis de índice que impedem incompatibilidade entre embeddings
- Provedores de LLM e de embeddings **plugáveis**
- **Automação com n8n** — *insights* de documentos, *retry*, idempotência e observabilidade

**Stack:** Python · FastAPI · SQLAlchemy 2 · PostgreSQL 16 + pgvector · Ollama (`llama3.2:3b`) · Vue 3 · TypeScript · Vite · Docker Compose · n8n

**Roadmap:** reranking por *cross-encoder* · *serving* com vLLM · curadoria de dataset e *fine-tuning* · agents e *tool calling*

---

## Experiência com sistemas privados

Além dos projetos públicos, desenvolvo sistemas corporativos privados envolvendo automação financeira, RH, faturamento, integrações, APIs e Inteligência Artificial. **Código e dados não são publicados por confidencialidade.**

O que esses sistemas cobrem, em capacidade técnica:

| Domínio | Natureza do trabalho |
|---|---|
| Automação financeira | Processamento e acompanhamento de pagamentos, integração bancária com mTLS e OAuth2, idempotência e trilha de auditoria |
| Integração corporativa | ERP, plataformas de BPM e serviços internos, com autenticação implementada à mão (OAuth 1.0a HMAC-SHA1, OAuth2, JWT, LDAP) |
| RH e recrutamento | Portal de vagas, leitura e triagem de currículos por LLM, score de aderência por vaga |
| Faturamento | Automação de processo e assistente de atendimento sobre API de mensageria, com guardrails de saída e *handoff* para humano |
| Contábil e fiscal | Motores de conferência diária sobre o ERP, entregando à equipe só o que exige decisão humana |
| Validação documental | Classificação de documentos com modelo de visão, calibrada sobre volume real |
| Dashboards operacionais | Posição consolidada e indicadores para gestão |
| IA aplicada a processo | RAG corporativo, agentes internos e automação orientada a eventos |

---

## Stack

**Backend** — Python · FastAPI · Node.js · Express · REST APIs · SQLAlchemy · Sequelize · JWT · processamento assíncrono

**Frontend** — Vue 3 · TypeScript · JavaScript · Vite · HTML · CSS · React · SPA e painéis administrativos

**Dados** — PostgreSQL · Oracle · SQL · pgvector · MongoDB

**IA** — RAG · LLMs · SLMs · Ollama · embeddings · *vector search* · *prompt engineering* · *grounded generation* · avaliação de RAG · reranking BM25 · TensorFlow · Keras · OpenCV · TFLite

**Automação e infraestrutura** — n8n · Docker · Docker Compose · Git · GitHub · webhooks · pipelines orientados a eventos · observabilidade

---

## Estudando agora

**vLLM** — *serving* de modelos, API compatível com OpenAI, inferência local, *throughput*, *batching*, concorrência, uso de GPU e VRAM, e comparação prática com Ollama. O FlowMind já foi arquitetado com provedor de LLM desacoplado justamente para receber isso sem reconstruir o pipeline de RAG.

**Fine-tuning** — estudando e preparando *pipelines* para curadoria de dataset, treino e avaliação. O alvo é comportamento, intenção, classificação e formato de resposta — **não** regra de negócio mutável, que muda mais rápido do que um modelo treinado consegue acompanhar.

---

## Pesquisa acadêmica

Mestrando em **Computação Aplicada**. É uma frente experimental, e fica deliberadamente separada dos sistemas em produção acima.

**Machine learning e deep learning** — CNN · ResNet · MobileNet · YOLO
**Visão computacional** — classificação de imagens · identificação de plantas daninhas
**Edge AI** — TFLite e inferência em dispositivo
**Sensores e sinais** — nariz eletrônico · análise de sinais · PCA · LDA · SVM

---

## Outros projetos públicos

**[Projeto-FullStack](https://github.com/1Rodrigo97/Projeto-FullStack)** — aplicação monolítica Node.js + Express + Vue + PostgreSQL: autenticação JWT, CRUD protegido, importação massiva de CSV (200 mil registros), paginação otimizada em SQL e SPA consumindo a API.

---

## Contato

**GitHub** · [1Rodrigo97](https://github.com/1Rodrigo97)
**LinkedIn** · [rodrigo-martins-198a32157](https://www.linkedin.com/in/rodrigo-martins-198a32157/)
**E-mail** · rodrigomartins246@gmail.com

---

<img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=1Rodrigo97&layout=compact&theme=tokyonight&hide_border=true" alt="Linguagens mais usadas" height="150">
<img src="https://github-readme-stats-sigma-five.vercel.app/api?username=1Rodrigo97&show_icons=true&theme=tokyonight&hide_border=true&hide_title=true" alt="Estatísticas do GitHub" height="150">
