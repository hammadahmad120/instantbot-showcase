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

<img width="1426" height="1009" alt="live-grounded-chat" src="https://github.com/user-attachments/assets/49f5566f-da00-49f7-8a6f-c7b064a5e060" />
<img width="879" height="1009" alt="doc-scout-result" src="https://github.com/user-attachments/assets/55c58023-f7dc-4d25-aa19-f68ef549dd32" />
<img width="1825" height="1009" alt="Performance-monitoring" src="https://github.com/user-attachments/assets/8ba1b5b4-30d3-4aee-80ff-e40b07b78ed5" />
<img width="1248" height="1009" alt="quick-web-widget-creation" src="https://github.com/user-attachments/assets/5bfdfcb6-6a62-45e2-b98a-f2139a4bc42e" />
<img width="780" height="1009" alt="whatsapp-integration-screen" src="https://github.com/user-attachments/assets/53f7da98-3172-44d3-a45c-5b8b4d9767ae" />
<img width="1060" height="1009" alt="RAG-Document-pipeline" src="https://github.com/user-attachments/assets/d04d1cb8-76e2-47f7-bf73-4985e79bf7d4" />





