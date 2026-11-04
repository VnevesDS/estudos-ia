# estudos-ia

Meu repositório de estudo de **Engenharia de IA aplicada a dados**: 70 dias de estudo (nov/2026 a fev/2027), de segunda a sexta, 1h30 a 2h por dia.

O plano junta duas ementas (Engenharia de Software em IA Aplicada e MBA AI Engineering & Multi-Agents) e foca em usar IA no trabalho com dados: analytics, finanças e relatórios. A prática é em Python.

## Trilha

| Semana | Tema | Projeto |
|---|---|---|
| 01 | Fundamentos de IA e Machine Learning | Notebook "ciclo completo": dados → treino → validação → inferência |
| 02 | LLMs por dentro | Comparativo de modelos local x API |
| 03 | APIs de IA e Prompt Engineering | Classificador de textos de negócio com saída JSON |
| 04 | Multimodal e IA aplicada a dados | API `/explicar-variacao` com FastAPI |
| 05 | RAG I: embeddings e busca semântica | "Pergunte à documentação" com citação de fontes |
| 06 | RAG II: qualidade e avaliação | RAG v2 com busca híbrida, reranking e evals |
| 07 | Tool use e agentes | Agente analista sobre um banco de dados |
| 08 | MCP (Model Context Protocol) | MCP server de dados da área |
| 09 | Memória, contexto e LangGraph | Agente v2 com memória e aprovação humana |
| 10 | Multi-agentes e arquitetura | Design doc (ADR) de um sistema de IA |
| 11 | IA para gestão de projetos | Status report automático + Monte Carlo de prazos |
| 12 | AI Operations | Pipeline de evals no CI |
| 13 | Fine-tuning e Responsible AI | Mini fine-tuning com LoRA |
| 14 | Capstone | Solução completa com demo |

## Como rodar

Requer [uv](https://docs.astral.sh/uv/) (gerenciador de ambientes e pacotes Python).

```bash
git clone https://github.com/VnevesDS/estudos-ia.git
cd estudos-ia
uv sync                      # cria o .venv e instala as dependências
uv run jupyter lab           # abre o Jupyter no navegador
```

Chaves de API ficam num arquivo `.env` (copie de `.env.example`). Ele está no `.gitignore` e nunca deve ir para o GitHub.

## Estrutura

```
estudos-ia/
├── linha-do-tempo.md        # Dia 1: história da IA
├── semana-01/               # notebooks e código de cada semana
├── pyproject.toml           # dependências do projeto
└── .env.example             # modelo das variáveis de ambiente
```
