# About me

I work at the intersection of large programs, stakeholders, and technology. I have 20+ years of experience in the United Nations system, spanning program coordination, project management, and stakeholder engagement.

These are hands-on applied AI projects. I build them to understand how AI systems work in practice: where they're reliable, where they fail, and what it takes to put guardrails around them.

## Projects

### [AI Content Automation with Human-in-the-Loop Approval](https://github.com/bettes777/linkedin-autogen)
Four AI agents research, draft, review, and score LinkedIn posts for a fictional fintech brand. An n8n workflow publishes only high-confidence drafts and sends everything else to human review in Slack, with dry-run mode, error alerts, and a full run log.
`n8n` `AutoGen` `FastAPI` `Azure OpenAI` `Slack`

### [Multi-Agent Research Assistant with Smart Source Routing](https://github.com/bettes777/agentic-rag-router-retriever)
A Router agent decides whether each question should be answered from a PDF knowledge base, from live web search, or directly by the model, and a Retriever agent answers it, with every step logged. Checking the answers against the source document caught a factual error, a reminder that fluent output isn't the same as grounded output.
`CrewAI` `Azure OpenAI` `Tavily` `FAISS`

### [AI Document Q&A Assistant (RAG Pipeline)](https://github.com/bettes777/rag-pdf-pipeline)
Answers questions across 159 pages of AI governance and digital strategy reports (NIST, UN, UNDP) and returns the source passages behind each answer. Reviewing those sources showed that all retrieved passages came from a single report, a retrieval-balance problem that a polished answer had hidden.
`LangChain` `FAISS` `Azure OpenAI` `Python`

## What I focus on

- **Turning a business need into a working AI workflow**, from requirements through to testing
- **Evaluation and guardrails:** confidence thresholds, human review, checking answers against sources
- **Responsible AI:** how governance frameworks such as the NIST AI Risk Management Framework translate into practical design choices

*All three projects were built as course-end projects for the Post Graduate Program in Applied Agentic AI (Virginia Tech & Simplilearn).*
