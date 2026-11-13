## InstantBot: AI knowledge assistant & document intelligence suite

Multi-tenant AI suite I created and built end to end.

### Products
- **Knowledge Assistant:** grounded, citation-backed answers over company documents
- **Document Scout:** screens and ranks documents against requirements with
  source-quoted verification (used internally by HR to screen CVs)

### Channels & integrations
The same assistant, knowledge base, and guardrails serve every channel:

- **Web chat:** full chat interface with cited sources for each answer
- **Embeddable widget:** drops into any existing website, so a company can put
  the assistant on its own pages
- **WhatsApp:** users ask questions in a normal WhatsApp conversation and get
  the same grounded answers

Each tenant gets isolated data (row-level security), rate limits, and usage
quotas that apply across all three channels.

### Under the hood
**Pipeline:** Ingest → Embed → Hybrid retrieve → Rerank → Ground → Answer
**Stack:** Python · Node.js · PostgreSQL + pgvector · RAG · guardrails · MCP
**Evaluation:** recall, MRR, hit@k, and latency tracked per release

Source is private. [Read the case study](https://www.hammadahmad.me/projects/instantbot),
or reach out and I'll walk you through the architecture.

<img width="879" height="1009" alt="doc-scout-result" src="https://github.com/user-attachments/assets/4ed389e6-a4a7-4b3f-8b6b-b87b0d5d3fb5" />
