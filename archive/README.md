# Archive

Les contributions qu'on **ne veut plus faire vivre au premier plan**, sans les effacer.

Git garde déjà toute l'histoire. L'archive sert les humains (et la Carte) : alléger [`../idees/`](../idees/), [`../points-de-vue/`](../points-de-vue/), etc., tout en laissant une trace **lisible** de ce qu'on a mis de côté — et pourquoi.

## Quand archiver ?

- L'idée est **abandonnée**, **fusionnée** dans une autre, ou **remplacée**.
- Le débat est **clos** sans suite, ou **obsolète** (le sujet a bougé).
- On veut **décongestionner** la Carte et la sidebar, sans perdre la mémoire.

Ce n'est **pas** une poubelle morale : une graine archivée peut être rouverte (on la ressort du dossier).

## Comment archiver (petit pas)

1. Déplacer le fichier vers le sous-dossier qui correspond à son étape :
   - idée → [`idees/`](idees/)
   - débat → [`points-de-vue/`](points-de-vue/)
   - synthèse → [`syntheses/`](syntheses/)
   - slogan → [`slogans/`](slogans/)
   - décision retirée / remplacée → [`decisions/`](decisions/)
2. En tête du fichier, ajouter ou mettre à jour :
   - **Statut** : `archivée`
   - **Archivée le** : `AAAA-MM-JJ`
   - **Motif** (une phrase) : abandon · fusionnée dans … · remplacée par … · hors-sujet temporaire
   - **Remplacée / fusionnée dans** : lien Markdown si pertinent
3. Mettre à jour les index : [`../CARTE.md`](../CARTE.md), le `README.md` du dossier d'origine, et [`../_sidebar.md`](../_sidebar.md).
4. Ouvrir une **Pull Request** (comme toute contribution).

## Règles

- **On ne delete pas** le contenu pour « faire propre » : on déplace.
- Les liens cassés se réparent dans la même PR (ou on laisse un stub d'une ligne dans l'ancien chemin — à éviter si possible).
- L'archive n'est **pas** indexée comme « en cours » sur la Carte.

## Voir aussi

- Décision : [`../decisions/0002-archivage-vues-et-noyau-slogans.md`](../decisions/0002-archivage-vues-et-noyau-slogans.md)
- Processus : [`../workflow/processus.md`](../workflow/processus.md)
