# memento

RAG local sur les *Pensées* de Marc Aurèle (traduction Jules Barthélemy-Saint-Hilaire, 1876, domaine public).

« Une citation pour ma situation » : recherche sémantique et hybride sur les pensées, éval mesurée (rappel@5, MRR), serveur MCP `cite_me`.

Projet test de [mr-orchestrator](../mr-orchestrator) : il est construit par des agents, ticket par ticket. Le tag `baseline-v0` marque l'état de départ des runs.

```bash
uv sync
uv run pytest
```
