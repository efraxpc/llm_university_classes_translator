# LLM Project — Efrain INFNET

Projeto prático de Large Language Models desenvolvido para o curso INFNET.  
Cobre desde chamadas básicas a APIs até pipelines completos de RAG.

## Estrutura

| Notebook | Tema |
|---|---|
| `c01_modelos_llm.ipynb` | Modelos LLM — APIs, comparação de modelos, uso de tokens |
| `c02_prompting.ipynb` | Prompting — zero-shot, few-shot, chain-of-thought, personas |
| `c03_embeddings_busca.ipynb` | Embeddings e busca semântica com FAISS |
| `c04_inferencia_local_ou_remota.ipynb` | Inferência local (Ollama, HuggingFace) vs. remota (API) |
| `c05_rag_pipeline.ipynb` | Pipeline RAG completo com avaliação de fidelidade |

## Configuração

### 1. Ambiente virtual

```bash
python -m venv .venv
source .venv/bin/activate        # Linux/macOS
.venv\Scripts\activate           # Windows
pip install -r requirements.txt
```

### 2. Variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
ANTHROPIC_API_KEY=sua_chave_aqui
OPENAI_API_KEY=sua_chave_aqui   # opcional
```

### 3. Inferência local (opcional — C04)

```bash
# Instalar Ollama: https://ollama.com
ollama serve
ollama pull llama3.2
```

### 4. Executar os notebooks

```bash
jupyter lab
```

## Dependências principais

- **anthropic** — API Claude
- **sentence-transformers** — geração de embeddings
- **faiss-cpu** — índice vetorial
- **ollama** — inferência local
- **transformers / torch** — modelos HuggingFace

## Autor

Efrain Colmenares — INFNET 2026
