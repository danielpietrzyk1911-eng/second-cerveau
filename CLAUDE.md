# Second cerveau de Daniel — règles pour Claude

Ce dépôt est le coffre Obsidian de Daniel, synchronisé par le plugin Obsidian Git.
C'est ta base de connaissances de référence : consulte-la avant de répondre à une
question qui touche à ses projets, ses restaurants, ses préférences ou ses décisions,
et mets-la à jour quand tu apprends quelque chose de durable.

## Organisation (méthode PARA)

- `00 Inbox/` : notes brutes à trier. Tout ce qui n'a pas encore de place va ici.
- `10 Projets/` : projets en cours, avec un objectif et une fin (ex. refonte du site Artusi).
- `20 Domaines/` : responsabilités durables (chaque restaurant, marketing, finances…).
- `30 Ressources/` : connaissances de référence (prompts qui marchent, fournisseurs, outils…).
- `40 Archives/` : projets terminés, notes obsolètes.
- `_claude/` : espace de Claude (journal, index).

## Règles d'écriture

1. **Chercher avant de créer** : si une note sur le sujet existe, la compléter plutôt que d'en créer une nouvelle.
2. **Une note = une idée**, titre clair en français, nom de fichier = titre (`Nom de la note.md`).
3. **Toujours relier** : chaque note créée ou modifiée contient au moins un lien `[[...]]` vers une note existante.
4. **En-tête YAML** sur chaque note créée :
   ```yaml
   ---
   tags: [projet|domaine|ressource, ...]
   créé: AAAA-MM-JJ
   maj: AAAA-MM-JJ
   source: claude | daniel
   ---
   ```
5. **Ne jamais supprimer** une note de Daniel : déplacer dans `40 Archives/` si obsolète.
6. **Ne jamais réécrire** le texte de Daniel : ajouter une section `## Ajouts de Claude (AAAA-MM-JJ)` en bas.
7. **Pas de secrets** (mots de passe, clés API, codes) dans le coffre.

## Après chaque modification

- Ajouter une ligne dans `_claude/Journal.md` : date, notes touchées, en une phrase ce qui a changé.
- Mettre à jour `_claude/Index.md` si une note importante est créée.
- Commit en français (`Ajout : …`, `Mise à jour : …`), puis push sur `main`.
