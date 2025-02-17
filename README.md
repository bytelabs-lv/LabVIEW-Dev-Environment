# Template repository per progetti LabVIEW
Questo repository serve come template per progetti di tipo LabVIEW.

## Contenuto
* Il .gitignore evita già di sincronizzare file dinamici di labview (come gli aliases e gli lvlps)
* Il .gitattributes evita merge automatici su alcuni files come gli lvproj, che altrimenti vengono trattati ed uniti come file xml, rompendoli.

## Istruzioni
1. Scarica l'ultima release (scaricando lo zip, non facendo clone)
2. Rinomina la cartella come ti fa più comodo ed inizializza il git repository (comando `git init` da command line).
3. Crea un repository vuoto su Bitbucket (non aggiungere .gitignore o README altrimenti andranno in conflitto).
4. Aggiungi il remote che ti serve per il tuo progetto (comando `git remote add origin https://path/of/repo.git`).
5. Copia o crea i file del progetto nella cartella appena ottenuta.
6. Sei pronto per fare add, commit e push dei file che vuoi sincronizzare.