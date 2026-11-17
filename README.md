## From large programs to applied AI
I work at the intersection of large programs, stakeholders, and technology. I have 20+ years of experience in the United Nations system, spanning program coordination, project management, and stakeholder engagement.

The projects below are hands-on applied AI projects. I build them to understand how AI systems work in practice: where they're reliable, where they fail, and what it takes to put guardrails around them.

## Projects

### [AI Content Automation with a Human Review Gate](https://github.com/bettes777/linkedin-autogen)
Four AI agents propose ideas, draft, review, and score LinkedIn posts for a fictional fintech brand. An automated workflow, built in n8n (a workflow automation tool similar to Zapier), is designed to publish only drafts that score above a confidence threshold and to send the rest to a person for review in Slack. It was tested end to end in dry-run mode, where every draft goes to Slack and nothing is posted publicly; live publishing has not been tested. It also has error alerts and a log of every run.
`n8n` `AutoGen` `FastAPI` `Azure OpenAI` `Slack`

### [Multi-Agent Research Assistant with Smart Source Routing](https://github.com/bettes777/agentic-rag-router-retriever)
A Router agent decides whether each question should be answered from a PDF knowledge base, from live web search, or directly by the model, and a Retriever agent answers it, with every step logged. Checking the answers against the source document caught a factual error, a reminder that fluent output isn't the same as grounded output.
`CrewAI` `Azure OpenAI` `Tavily` `FAISS`

### [AI Document Q&A Assistant (RAG Pipeline)](https://github.com/bettes777/rag-pdf-pipeline)
Answers questions across 159 pages of AI governance and digital strategy reports (NIST, UN, UNDP) and returns the source passages behind each answer. Reviewing those sources showed that all retrieved passages came from a single report, a retrieval-balance problem that a polished answer had hidden.
`LangChain` `FAISS` `Azure OpenAI` `Python`

### [AI Advisory Team for Startup Founders](https://github.com/bettes777/startup-accelerator-agents)
From one input, the startup's sector, three AI agents (a researcher, a funding advisor, and a pitch coach) work as a team to produce a pitch deck outline. They share notes through a common memory, send each other questions, and review each other's drafts, coordinated with LangGraph (a framework for building multi-step AI agent workflows). The agents are instructed to label every unverified figure for checking, which held in the demo run (run without web search, so all figures came from the model and were labelled). A limit on review rounds keeps the workflow predictable: when reviewers still had concerns at the limit, the output recorded their open feedback for the founder instead of hiding it.
`LangGraph` `Azure OpenAI` `Python` `Multi-agent systems`

## What I focus on

- **Turning a business need into a working AI workflow**, from requirements through to testing
- **Evaluation and guardrails:** confidence thresholds, human review, checking answers against sources
- **Responsible AI:** how governance frameworks such as the NIST AI Risk Management Framework translate into practical design choices

