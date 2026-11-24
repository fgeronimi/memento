# memento

Moteur RAG local sur les *Pensées* de Marc Aurèle, traduction Barthélemy-Saint-Hilaire (1876, domaine public). Projet test piloté par `mr-orchestrator` : la spec est dans `mr-orchestrator/docs/brief.md`.

## Règles

- Aucun modèle payant : embeddings et génération tournent en local.
- Une pensée = un document, identifié `livre.pensée` en chiffres romains (`VI.1`).
- Une citation renvoyée doit exister mot pour mot dans le corpus.
- Toute modification de l'ingestion, des embeddings ou de l'index est une zone sensible : revue humaine obligatoire.
- Pendant un run, travailler sur une branche issue de `run/NNN` et ouvrir la PR vers `run/NNN`, jamais vers `main`.

## Commandes

- `uv sync` : installer
- `uv run pytest` : tests
- L'éval (rappel@5, MRR) vivra dans `eval/` et devra tourner en une commande.

## Définition de fini

- Tests ajoutés pour tout code ajouté, `uv run pytest` vert.
- Le score d'éval ne baisse pas, ou la baisse est expliquée dans la PR.
