| Dr. | Y. Mekouar | –   | ESISA |     |     |              | DevOps | et IA      |         |              | Annee 2026–2027  |         |
| --- | ---------- | --- | ----- | --- | --- | ------------ | ------ | ---------- | ------- | ------------ | ---------------- | ------- |
|     |            |     |       |     |     |              |        | TP 1 :     | Depot,  | Notion       | et Environnement |         |
|     |            |     |       |     |     | Master IS2IA | –      | 5eme Annee | – Duree | : 3 h (cours | 1 h 30 + TP      | 1 h 30) |
Objectif
Creer le depot GitHub du fil rouge, le tableau Notion et un environnement reproductible (Codes-
| paces     | ou Docker   |                 | local).       |     |        |       |        |         |     |     |     |     |
| --------- | ----------- | --------------- | ------------- | --- | ------ | ----- | ------ | ------- | --- | --- | --- | --- |
| Objectifs |             | d’apprentissage |               |     |        |       |        |         |     |     |     |     |
|           | — Expliquer |                 | les principes |     | DevOps | et la | boucle | Dev-Ops |     |     |     |     |
— Decrire les quatre metriques DORA et leur lien avec la performance
— Appliquer Scrum et Kanban pour organiser un backlog dans Notion
|     | — Concevoir |     | l’architecture |     | cible | du fil rouge | et  | un plan | de sprint |     |     |     |
| --- | ----------- | --- | -------------- | --- | ----- | ------------ | --- | ------- | --------- | --- | --- | --- |
— Deployer l’environnement de travail : depot GitHub et Codespaces ou Docker local
Prerequis
|             | — Compte | GitHub |      | (GitHub       | Education  |      | recommande) |           |     |     |     |     |
| ----------- | -------- | ------ | ---- | ------------- | ---------- | ---- | ----------- | --------- | --- | --- | --- | --- |
|             | — Git,   | Python | 3.12 | ou Docker     | installes, |      | ou un       | Codespace |     |     |     |     |
|             | — Compte | Notion |      | gratuit       |            |      |             |           |     |     |     |     |
| Deroulement |          | (90    | min  | : 15/45/20/10 |            | min) |             |           |     |     |     |     |
Voir les etapes ci-dessous; chronometrer chaque etape. Etape du fil rouge
S1 : depot GitHub, README, tableau Notion (backlog, sprint, retro) et roles. Etapes detaillees
1. Creerledepot:Undepotparequipe,nomcapstone-devops-NOMEQUIPE.AjouterREADME
|     | et .gitignore |     | Python. |     |     |     |     |     |     |     |     |     |
| --- | ------------- | --- | ------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
2. Recuperer le starter : Copier le contenu de capstone-starter/ dans le depot, puis verifier le
|     | fonctionnement |                          |      | local.           |           |                    |                      |     |     |     |     |     |
| --- | -------------- | ------------------------ | ---- | ---------------- | --------- | ------------------ | -------------------- | --- | --- | --- | --- | --- |
|     | python         | -m                       | venv | .venv            | && source | .venv/bin/activate |                      |     |     |     |     |     |
|     | pip            | install                  | -r   | requirements.txt |           | -r                 | requirements-dev.txt |     |     |     |     |     |
|     | uvicorn        | app.main:app             |      |                  | --reload  |                    |                      |     |     |     |     |     |
|     | curl           | -s localhost:8000/health |      |                  |           |                    |                      |     |     |     |     |     |
3. Environnement reproductible:OuvrirledepotdansGitHubCodespaces(ouDockerlocal).
|     | Verifier | python | –version |     | et git | –version. |     |     |     |     |     |     |
| --- | -------- | ------ | -------- | --- | ------ | --------- | --- | --- | --- | --- | --- | --- |
4. Tableau Notion : Creer la base Kanban : Backlog, Pret, En cours, En revue, Termine;
|     | proprietes |     | Semaine, | Assigne, |     | Priorite, | Lien | PR. |     |     |     |     |
| --- | ---------- | --- | -------- | -------- | --- | --------- | ---- | --- | --- | --- | --- | --- |
5. Roles et definition of done : Attribuer les 4 roles, ecrire la definition of done (tests verts,
|          | revue | faite,  | doc    | a jour). |     |     |     |     |     |     |     |     |
| -------- | ----- | ------- | ------ | -------- | --- | --- | --- | --- | --- | --- | --- | --- |
| Resultat |       | minimal | viable |          |     |     |     |     |     |     |     |     |
Depot cree, API qui repond sur /health, tableau Notion avec 5 cartes.
Plan B
Brancher les equipes sur la branche starter du depot de reference et passer a l’etape Notion.
Exercices
|     | 1. Cloner   | le     | depot        | et lancer | l’API       |         |           |           |     |     |     |     |
| --- | ----------- | ------ | ------------ | --------- | ----------- | ------- | --------- | --------- | --- | --- | --- | --- |
|     | 2. Ecrire   | 5 user | stories      | dans      | Notion      |         |           |           |     |     |     |     |
|     | 3. Definir  | la     | definition   | of        | done        |         |           |           |     |     |     |     |
|     | 4. Mesurer  | le     | lead         | time de   | la premiere | carte   |           |           |     |     |     |     |
|     | 5. Exercice |        | IA : backlog |           | genere      | par IA, | puis revu | a la main |     |     |     |     |
1

| Dr. Y. Mekouar | – ESISA           |        |            | DevOps et IA   |                | Annee 2026–2027 |
| -------------- | ----------------- | ------ | ---------- | -------------- | -------------- | --------------- |
| Regle          | pour l’exercice   | IA     |            |                |                |                 |
| L’IA           | propose, l’humain | valide | – toujours | executer lint, | tests et plan. |                 |
Pieges frequents
— Codespaces : quota gratuit limite, arreter le Codespace apres usage
| — Ne      | jamais committer | de          | fichier .env  | ni de jeton |     |     |
| --------- | ---------------- | ----------- | ------------- | ----------- | --- | --- |
| — Un      | depot par        | equipe, pas | par personne  |             |     |     |
| Livrables | et bareme        | (/20)       |               |             |     |     |
| — Lien    | du depot         |             |               |             |     |     |
| — Capture | du tableau       | Notion      |               |             |     |     |
| — Fichier | ROLES.md         | avec        | la definition | of done     |     |     |
— Qualite : etapes reproductibles (README), commits propres, aucun secret
Depot GitHub
labs/week-01-culture-devops/README.md
2